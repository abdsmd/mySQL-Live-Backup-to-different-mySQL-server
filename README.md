## You Can Choose VPS from DigitalOcean
[![DigitalOcean Referral Badge](https://web-platforms.sfo2.cdn.digitaloceanspaces.com/WWW/Badge%201.svg)](https://www.digitalocean.com/?refcode=4ef7bcd8895a&utm_campaign=Referral_Invite&utm_medium=Referral_Program&utm_source=badge)




# mySQL-Live-Backup-to-different-mySQL-server
How to live backup of mySQL server to remote mySQL server



# Full Database
``` mysqldump -uroot -pPassword DATABASE_NAME | ssh root@REMOTE_IP mysql -uroot -pPassword  DATABASE_NAME ```


# Few Table  

``` mysqldump -uroot -pPassword DATABASE_NAME TABLE1 TABLE2 TABLE3 | ssh root@188.34.197.112  mysql -uroot -pMasm@#$ DATABASE_NAME ```


# Full Raw Data Transfer Fastest

``` cd /var/lib/mysql/ && scp -r ./*  root@REMOTE_IP:/var/lib/mysql/ ```
