##  Basic work with files

- Create directory test1

```console
mkdir test
```

- Create file test1.txt inside the test1 directory.

```console
touch test1.txt
```

-   Create copy of folder test1 with name test2.  

```console
cp -r /home/mininoobass/Desktop/GIT/test_ggs/test1 test2
```

-    Delete file test1.txt inside test2 directory.

```console
rm test1.txt
```

-    Rename test2 folder into directory_without_file



-    Insert 'test1' text into test1/test1.txt file.

-    print the text from the test1/test1.txt file.

-    Insert 'test2' into the end of test1/test1.txt file.

-    print the text from the test1/test1.txt file.

- check the size of test1 directory

## Permissions

-   Create test directory and block access for all to it.

-   Try to remove that directory.


-    Create simple script which prints current date. Try to execute it.


## Log checking

-  Count lines in the file test.txt.

```console
wc -l test.txt
```

- Show last 3 lines from the test.txt file. 

```console
tail -n 3 test.txt
```

-  Hom many uniq IP addresses accessed the website ? 

```console
grep -E -o "^[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}" test.txt | sort -n | uniq -c | wc -l
```

-  IP address with most requests.

```console
grep -E -o "^[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}" test.txt | sort -n | uniq -c | sort -n | tail -n 1
```

-  Top 3 IP addresses by amount of POST requests.

```console
grep -E post test.txt > testpost.txt

grep -E -o "^[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}" testpost.txt | sort -n | uniq -c | sort -n | tail -n 3
```

-  Which IP addresses received 403 error ? 


- Task with * . Write script to show which pages Google checked from the website 

## Replace

Replace IP address with most requests on 127.0.0.1 in test.txt file 
