# SHEET -5 – I/O REDIRECT,FILTERS(TEE,GREP,WC)
## I/O Redirect
## Redirecting standard o/p and error
### 1. Create a file called output.txt that contains the output of the date command Note : run date cmd in the terminal and observe the o/p.
![alt text](image.png)
### 2. Append the current user’s name to a file called output.txt ( use whoami)
![alt text](image-1.png)
### 3. Append the host name to a file called output.txt ( use hostname)
![alt text](image-2.png)
### 4. Attempt to list a non-existent directory and redirect the error message to error.log
![alt text](image-3.png)
### 5. Run a cmd to get output and error and redirect only the output to file and display the error
![alt text](image-4.png)
### a. Use ls -l existingdir non-existentdir → e.g. ls -l CEO dir1 2>&1 > error.log
![alt text](image-5.png)
### b. Cat existingfile non-existentfile
![alt text](image-6.png)
### 6. Run a cmd to get output and error and redirect only the error to file and display the output
![alt text](image-7.png)
### 7. Run a cmd to get output and error and redirect both to combined.txt
![alt text](image-8.png)
### a. Use ls -l existingdir non-existentdir → e.g. ls -l CEO dir1  > combined.txt 2>&1
![alt text](image-9.png)
### b. Cat existingfile non-existentfile Redirecting standard i/p
![alt text](image-10.png)
### 8. Create a file with numbers. Read the file using cat cmd .
![alt text](image-11.png)
### 9. Read the same file using cat and i/p redirect e.g cat < file.txt
![alt text](image-12.png)
### 10.  Read the file  /etc/passwd file and display only last 4 lines using i/p redirect and o/p to a file 
![alt text](image-13.png)
# Filters or text processor cmds.
##    1. Tee
![alt text](image-14.png)
###    a. To output.txt echo “Hello world”  using tee cmd
![alt text](image-15.png)
###    b. Run the cmd uname -a and append it to output.txt using tee -a cmd
![alt text](image-16.png)
###    c. Run tac filename | tee Newfile | tac and observe. (tac is opposite of cat)
![alt text](image-17.png)
##    2. Grep
###    a. Create a text file named sample.txt with the following content
###    Hello World
###    Welcome to the world of Linux
###    Learning commands is fun
![alt text](image-19.png)
###    b. Use grep cmd to find word ‘world’
![alt text](image-18.png)
###    c. Use grep cmd to find word ‘world’ case-insensitive
![alt text](image-20.png)
###    d. Use grep to count how many lines contain the word "Linux" in sample.txt (use grep -c “keyword” filename)
![alt text](image-21.png)
###    e. Use grep to display lines from sample.txt that do not contain the word "fun” (option -v)
![alt text](image-22.png)
###    f. Use egrep (extended grep) to find world and fun from sample.txt
![alt text](image-23.png)
###    g. Use ls -l | grep “keyword”
![alt text](image-24.png)
###    h. Cat /etc/passwd | grep “yourname”
![alt text](image-25.png)
###    i. Create a directory named test_dir and place sample.txt and more_sample.txt inside it.
![alt text](image-28.png)
###    Use grep to search for the word "World" recursively in the directory using grep -r "World" test_dir/
![alt text](image-27.png)
###    j. Try out the options grep -An , grep -Bn and grep -Cn
![alt text](image-29.png)
##    3. Sort
###    i. Create a file with some contents and perform the following
![alt text](image-31.png)
###    ii. Sort Filename , sort -r Filename ,sort -f filename ( -f = ignore case)
![alt text](image-30.png)
![alt text](image-32.png)
![alt text](image-33.png)
###    iii. Sort -k1 Filename (display column 1)
![alt text](image-34.png)
###    iv. Sort -nk3 Filename (sort numeric data and display col 3)
![alt text](image-35.png)
###    v. Sort -u Filename (sort and uniq)
![alt text](image-36.png)
###    vi. Ls -l | sort -k9 | uniq
![alt text](image-37.png)
###    vii. Use cat file1 file2 | sort (enter some relevant text in file1 and file2)
![alt text](image-38.png)
##  4. Uniq
###    i. Create a file with some duplicate contents and perform the following
###    ii. Uniq filename
![alt text](image-39.png)
###    iii. Uniq -c filename
![alt text](image-40.png)
###    iv. Use it with sort cmd and redirect the o/p to a file. (sort filename | uniq > filename)
![alt text](image-41.png)
##    5. WC
###    i. Find the no of lines ,no of words and no. of chars in a file of your choice using wc cmd
###    using wc filename ,wc -l ,wc -w ,wc -m
![alt text](image-42.png)
##    6. Cut
###    i. Create a text file named data.txt with the following content
###    John,25,Engineer
###    Alice,30,Designer
###    Bob,22,Developer
###    Charlie,28,Manager
![alt text](image-43.png)
###    ii. Use cut to extract and display the first field.use -d and -f option
![alt text](image-44.png)
###    iii. Use cut to extract and display the names and ages (first and second fields)
![alt text](image-45.png)
###    iv. Use cut to display the first 5 characters of each line in data.txt
![alt text](image-46.png)
###    v. Run ls -l | cut -d “ ” -f 9 |sort |uniq
![alt text](image-47.png)
###    vi. Use cut to extract the username in /etc/passwd file
![alt text](image-48.png)
##     7. Awk
###    i. awk ‘{print $1}’ file = List 1st field from a file
![alt text](image-49.png)
###    ii. ls –l | awk ‘{print $1,$3}’ = List 1 and 3rd field of ls –l output
![alt text](image-50.png)
###    iii. ls –l | awk ‘{print $NF}’ = Last field of the output
![alt text](image-51.png)
###    iv. awk '/keyword/ {print}' file = Search for a specific word
![alt text](image-52.png)
###    v. echo "Hello Tom" | awk '{$2="Adam"; print $0}‘ = Replace Tom with Adam
![alt text](image-53.png)