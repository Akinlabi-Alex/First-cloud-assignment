A.  Using absolute path:        
           cd /home/altschool/test

B.  Using relative path
           cd test 

C.  echo 'Hello A' > /home/altschool/misc/FileA

D.  Inside Misc directory
           touch fileB 
           then, vi fileB
           click the I (insert) button and write your dummy content
           click esc button after writing the dummy content
           click shift colon (:), wq to save and exit...Press enter

 E. To copy contents of fileA into fileC,
           cp misc/fileA misc/fileC

 F. To move contents of fileB into fileD
           mv misc/fileB misc/fileD

 G. To create a tar archieve called misc.tar
            sudo tar -cvf misc.tar misc
       After creation, click ls  from the home directory (/home/altschool) to check if the file has been created

 H. To compress the tar archieve to create misc.tar.gz file
            sudo gzip misc.tar
       After creation, click ls from the home directory (/home/altschool) to check if the file has been created 

 I. To create a user and force the user to change his/her password upon login
   - to create a user and set a password 
            sudo useradd alex
            sudo passwd 
    - to force the user to change his/her password upon login
            sudo chage -d 0 alex
            then  click su alex and enter current password 
              (You will be forced to change password) 

  J. To lock a user
            sudo passwd -l alex

  K. To create a user with nologin shell
            sudo useradd kola -s /sbin/nologin
            click grep kola /etc/passwd 
   
  L. To disable password based authentication for ssh
            sudo vi /etc/ssh/sshd_config
        search for password authentication then type no if it is yes

  M. To disable root login for ssh
            sudo vi /etc/ssh/sshd_config
        search for PermitRootLogin then type no if it is yes    
        


       






 
