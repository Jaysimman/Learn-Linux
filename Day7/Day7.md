### 1. Create a directory named TestaclDir under your home directory with 755 permissions
![alt text](image-1.png)
### 2. Create a file named TestaclFile under your home directory.
![alt text](image-2.png)
### 3. Observe the permissions of dir and file created (ls -l /ls -ld)
![alt text](image.png)
### 4. Use getfacl cmd  to check the permissions of user and group.
![alt text](image-3.png)
### 5. Change the group of the file and dir to sports. (assuming you have a group named sports)
![alt text](image-4.png)
### 6. Add a user – Sachin to sports. (usermod -aG cmd)
![alt text](image-5.png)
### 7. Now use setfacl cmd on TestaclDir to give permission -rwx (7) for user Sourav
![alt text](image-6.png)
### a. Use setfacl -m u:username:permission file/dirname
![alt text](image-7.png)
![alt text](image-8.png)
### b. Use setfacl --no-mask -m u:username:permission file/dirname ( the grp permissions will not change)
![alt text](image-9.png)
### c. Check the acl s using getfacl
![alt text](image-10.png)
### d. Observe a + sign .
![alt text](image-11.png)
### e. Setfacl on TestaclDir  for group -Football with permissions -rwx (7)
![alt text](image-12.png)
### f. Check the acl s using getfacl
![alt text](image-13.png)
### g. Access the dir as Sourav and test the permissions before and after setting the acls.
![alt text](image-14.png)
![alt text](image-15.png)
### h. Access the dir as any user in grp Football and test the permissions before and after setting the acls.
![alt text](image-19.png)
![alt text](image-20.png)
![alt text](image-21.png)
![alt text](image-22.png)
### 8. Repeat 7. For file TestaclFile.
![alt text](image-16.png)
### 9. Remove the acl s using setfacl -x u/g :user/grp file/dirname and chk with getfacl cmd
![alt text](image-17.png)
### 10.  Remove all acls using setfacl -b file/dirname
![alt text](image-18.png)