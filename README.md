# google-dorks-notes

**popular dorks operators**

cache: cached version of any website
```
cache:example.com
```
Finding Vulnerable Webcams:
```
inurl:/view.shtml intitle:"Live View / - AXIS"
```
Finding Open Directories:
```
intitle:"Index of" inurl:/
```
Finding Vulnerable WordPress Sites:
```
inurl:/wp-content/uploads/
```
Finding Login Pages:
```
inurl:/login
```
Finding Configuration Files:
```
filetype:env intext:DB_PASSWORD
```
Finding Backup Files:
```
intext:"Index of /backup"
```
Finding SQL Injection Vulnerabilities:
```
intext:"You have an error in your SQL syntax" intext:password | pass | passwd
```
Finding Cross-Site Scripting (XSS) Vulnerabilities:
```
intitle:"XSS (Cross Site Scripting) Prevention Cheat Sheet"
```
Finding Open Redirect Vulnerabilities:
```
inurl:/redirect?url=
```
Finding Vulnerable Apache Tomcat Servers:
```
intitle:"Apache Tomcat" intext:"If you're seeing this, you've successfully installed Tomcat. Congratulations!"
```
Finding PHPInfo Files:
```
intitle:phpinfo "PHP Version" "Server"
```
Finding Git Configuration Files:
```
intitle:index of /.git/config
```
Finding Exposed API Keys:
```
filetype:json api_key
```
Finding Vulnerable CCTV Cameras:
```
intitle:"Live View / - AXIS" | inurl:view/view.shtml
```
Finding Open Elasticsearch Servers:
```
intitle:"Elasticsearch Status - Cluster"
```
Finding Open MongoDB Databases:
```
intitle:"MongoDB Status" "inMemory"
```
Finding Apache Status Pages:
```
intitle:"Apache Status" "Server uptime"
```
Finding phpMyAdmin Installations:
```
intitle:"phpMyAdmin" intext:"Welcome to phpMyAdmin"
```
Finding Network Devices:
```
intitle:"Network Print Server" inurl:hp/device/this.LCDispatcher
```
Finding Open FTP Servers:
```
intitle:"index of" inurl:ftp
```
