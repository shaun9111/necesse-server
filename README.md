# necesse-server
How to create a necesse server on oracle cloud for free. (https://www.oracle.com/ca-en/cloud/free/)

This will require some knowloegd of creating an instance on oracle cloud and how to open ports on oracle cloud. Those steps arent listed yet. If you want, you can try looking at this video below   
https://youtu.be/g7sP33QtuxM

If anyone wants to commit changes, I will check them and credit you in the readme file afterwards. 

## LINKS
1. https://www.putty.org/
2. https://filezilla-project.org/

### Instructions 

Once you have a vm up and running and you have SSH into it using putty or other similar program. use the putty terminal to run these commands.

1. sudo yum check-update
2. sudo yum update
3. sudo yum install jdk-19
4. copy server files to home/opc/necesse (https://necessegame.com/server/) with fila zilla or other ftp file uploader
5. chmod +x /home/opc/necesse/StartServer-nogui.sh
6. chmod +x /home/opc/necesse/jre/bin/java
7. open linux ports with commands below
8. sudo firewall-cmd --permanent --zone=public --add-port=14159/tcp
9. sudo firewall-cmd --permanent --zone=public --add-port=14159/udp
10. Open ports on instence subnet on oracle
11. sudo firewall-cmd --reload
12. ./StartServer-nogui.sh
