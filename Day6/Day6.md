### 1. Use which cmd to check the where are its executable files
### a. Which pwd
### b. Which passwd
### c. Which su
### d. Which mount
### e. Which gpasswd
![alt text](image.png)
### 2. ist all the files having special permission 4 – setuid
### a. Find /usr/bin -type f -perm -4000
![alt text](image-1.png)
### b. Use find to get all files with spl perm 2- setgid from /usr/bin
![alt text](image-2.png)
### 3. List all the directories having special permission 2 – setgid from / directory (use find / -type d -perm -2000)
![alt text](image-3.png)
### 4. Run ls -l /usr/bin/gpasswd and observe the permission (-rws-r-x-r-x)
![alt text](image-4.png)
### a. Run the same for passwd and sudo and chmod and observe.
![alt text](image-5.png)
### b. Run ls -l /usr/bin/locate and observe the permission (-rwx--s--x)
![alt text](image-6.png)
### c. Run ls -l /usr/bin/write and observe the permission (-rwxr-sr-x)
![alt text](image-7.png)
### d. Run ls -ld /tmp and observe the permission (drwxrwxrwt)
![alt text](image-8.png)
### 5. Set up a directory, owned by the group sports. (setGID -4)
![alt text](image-9.png)
### a. Members of the sports group should be able to create files in this directory.
![alt text](image-10.png)
### b. All files created in this directory should be group-owned by the sports group.
![alt text](image-11.png)
### i. Use (chmod g+s dir/filename) and also using octal values (chmod 2775 dir/filename)
![alt text](image-12.png)
### c. Users should be able to delete only their own user-owned files.
![alt text](image-13.png)
### d. Check if this works.
![alt text](image-14.png)
### e. Try removing the permissions also and checking(chmod g-s dir.filename)
![alt text](image-15.png)
### 6. Create files and try setting and removing setuid permissions (setUID -2) and chk using ls -l filename
### a. Chmod u+s filename
![alt text](image-16.png)
### b. Chmod u-s filename
![alt text](image-17.png)
### c. Chmod 4764 filename
![alt text](image-18.png)
### d. Chmod 0764 filename
![alt text](image-19.png)
### 7. Become root user and create a shared full permission dir
![alt text](image-20.png)
### a. Become user kevin and create files and dirs.
![alt text](image-21.png)
### b. Login as another user and delete the files created by kevin.
![alt text](image-22.png)
### c. Now set sticky bit to the shared dir (chmod +t dirname) / chmod 1777 dirname).
![alt text](image-23.png)
### d. Again, as kevin create dirs and files inside shared folder.
![alt text](image-24.png)
### e. Login as another user and delete the files created by kevin.
![alt text](image-25.png)