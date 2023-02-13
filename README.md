# necesse-server
How to create a server on oracle cloud for free
1. sudo yum check-update
2. sudo yum update
3. sudo yum install jdk-19
4. copy server files to home/opc/necesse (https://necessegame.com/server/) with fila zilla or other ftp file uploader
5. chmod +x StartServer-nogui.sh
6. chmod +x java
7. open linux ports
8. sudo firewall-cmd --permanent --zone=public --add-port=14159/tcp
9. sudo firewall-cmd --permanent --zone=public --add-port=14159/udp
10. Open ports on instence subnet on oracle
11. sudo firewall-cmd --reload
