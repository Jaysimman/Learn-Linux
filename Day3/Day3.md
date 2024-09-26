### 1. List all the files and directories in your user directory

![alt text](image.png)

### 2. Observe the permission for each file and directories.

![alt text](image-1.png)

### 3. For Directory give the following permission using chmod cmd 
###        a. VP Sales
###        i.  User – rwx
###        ii.  Group – r-x
###        iii.  Others – r- -
![alt text](image-2.png)
###        b. People
###        i.  User – r - -
###        ii.  Group – r- -
###        iii.  Others – r- -
![alt text](image-3.png)
###        c. Sales Rep
###        i.  User – r - -
###        ii.  Group – - - -
###        iii.  Others – r- -
![alt text](image-4.png)
### 4. For Directory give the following permission using chmod cmd using Numeric values
### a. Product Lead
### i.  User – -w-
### ii.  Group – rwx
### iii.  Others – rwx
![alt text](image-5.png)
### b. Senior Developer
### i.  User – rwx
### ii.  Group – rw-
### iii.  Others – --x
![alt text](image-6.png)
### c. Tech Lead
### i.  User – r - x
### ii.  Group – r- x
### iii.  Others – rwx
![alt text](image-7.png) 
### 5. For the following files change permissions using chmod cmd 
### a. abc1-xyz
### i.  User – r - x
### ii.  Group – r- x
### iii.  Others – r-x
![alt text](image-8.png)
### b. abc2-xyz
### i.  User – rwx
### ii.  Group – rwx
### iii.  Others – rwx
![alt text](image-9.png)
### c. abc3-xyz
### i.  User – - - -
### ii.  Group – - -x
### iii.  Others – r--
![alt text](image-10.png)

### 6. For the following files change permissions using chmod cmd (Numeric values)
### a. abc4-xyz
### i.  User – r - x
### ii.  Group – ---
### iii.  Others – --x
![alt text](image-11.png)
### b. abc5-xyz
### i.  User – r - x
### ii.  Group – r- x
### iii.  Others – r-x
![alt text](image-12.png)
### c. abc6-xyz
### i.  User – r - x
### ii.  Group – r- x
### iii.  Others – r-x
![alt text](image-13.png)

### 7. Create a file – SoftLinkTest under your user directory, input some text and cat it to display its contents.

![alt text](image-14.png)

### 8. Repeat the same for file – HardLinkTest.

![alt text](image-15.png)

### 9.  Create softlink for file SoftLinkTest uner /tmp directory using ln-s cmd

![alt text](image-16.png)

### 10. Create hardlink for file HardLinkTest uner /tmp directory using ln cmd

![alt text](image-17.png)

### 11. Check the inodes for each file and its link.

![alt text](image-18.png)

### 12. Update the file contents and observe the changes

![alt text](image-19.png)

### 13. Delete the files and observe the changes

![alt text](image-20.png)

### 14. Create a hard and soft link for a directory of your choice and record the results.

![alt text](image-21.png)

### 15. Use cp cmd to copy a directory of your choice into CEO directory. Try with empty as well as with sub directories.

![alt text](image-22.png)

### 16. Go to /var/log, display the contents of file messages using more and less, head and tail cmd.

![alt text](image-23.png)
![alt text](image-24.png)
![alt text](image-25.png)
![alt text](image-26.png)

### 17. Go to /bin, run cmd ls -l | more

![alt text](image-27.png)

### 18. Go to /bin, run cmd ls -l | less

![alt text](image-28.png)

### 19. Go to /bin, run cmd ls -l | head

![alt text](image-29.png)

### 20. Go to /bin, run cmd ls -l | tail

![alt text](image-30.png)

### 21. Run head and tail cmd to get specified number of lines displayed eg. head -5, tail -3 etc.

![alt text](image-31.png)
![alt text](image-32.png)

### 22. Understand the use of Pipe |.

#### Combining two commands to do work in parallel