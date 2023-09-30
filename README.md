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
# Dorks-for-directory-discovery

Common Directory Names:
```
inurl:(admin|manager|login|wp-login|cp|control|panel|phpMyAdmin|phpmyadmin|webadmin)
```
Listing Directory Contents:
```
intitle:"Index of" inurl:(admin|manager|uploads|files|data|backup|logs)
```
Configuration Files:
```
intitle:"Index of" intext:(config|configuration|settings|setup|conf|ini)
```
Backup and Log Directories:
```
intitle:"Index of" intext:(backup|log)
```
Temporary Files and Directories:
```
intitle:"Index of" intext:(tmp|temp|cache)
```
Scripts and Libraries:
```
intitle:"Index of" intext:(js|css|php|asp|aspx|cgi|pl)
```
Configuration and Settings Files:
```
intitle:"Index of" intext:(config|settings|conf|ini) filetype:(xml|yaml|json)
```
Database Backups:
```
intitle:"Index of" intext:(database|db|sql) intext:(backup|dump|sql|tar|gz)
```
Git Repositories:
```
intitle:"Index of" intext:.git
```
Apache Server Status Page:
```
intitle:"Apache Status" intext:"Server uptime" inurl:/server-status
```
PHPMyAdmin Installations:
```
intitle:"phpMyAdmin" intext:"Welcome to phpMyAdmin"
```
Open Tomcat Manager:
```
intitle:"Tomcat Server Administration" inurl:/manager/html
```
Open Jenkins Instances:
```
intitle:"Dashboard [Jenkins]" inurl:/login?from=%2F
```
Exposed Elasticsearch Indices:
```
intitle:"Elasticsearch Indices" inurl:/_cat/indices?v
```
Exposed Kibana Dashboards:
```
intitle:"Kibana" intext:"Welcome to Kibana" inurl:/app/kibana
```
Exposed Grafana Dashboards:
```
intitle:"Grafana" inurl:/login
```
Exposed Jupyter Notebooks:
```
intitle:"Jupyter Notebook" inurl:/tree
```
Exposed Splunk Instances:
```
intitle:"Splunk" intext:"Splunk" inurl:/en-US/account/login
```
Exposed Jira Instances:
```
intitle:"Jira" inurl:/login.jsp
```
Exposed Confluence Instances:
```
intitle:"Confluence" inurl:/login.action
```
Open phpMyAdmin Directories:
```
intitle:"phpMyAdmin" inurl:"main.php"
```
Open phpinfo() Pages:
```
intitle:"phpinfo()" intext:"PHP Version" filetype:php
```
Exposed CVS and SVN Directories:
```
intitle:"Index of" inurl:(CVS|SVN)
```
Open Web Shell Directories:
```
intitle:"Index of" intext:(shell|shells|webshell|php)
```
Exposed Backup and Configuration Files:
```
intitle:"Index of" intext:(backup|config|conf|settings|cfg|setup) filetype:(.bak|.zip|.sql|.xml|.json)
```
Exposed Log Files:
```
intitle:"Index of" intext:(log|logs) filetype:(.log|.txt)
```
Open Apache Configuration Files:
```
intitle:"Index of" inurl:apache/conf
```
Exposed GitLab Repositories:
```
intitle:"GitLab" inurl:/dashboard
```
Open Mercurial Repositories:
```
intitle:"Mercurial Repositories" inurl:.hg/store
```
Exposed Subversion Repositories:
```
intitle:"TortoiseSVN" inurl:"filelistbox.cgi"
```
Open Microsoft SharePoint Sites:
```
intitle:"SharePoint" intext:"Sign in" inurl:/_layouts/
```
Exposed Ruby on Rails Config Files:
```
intitle:"Dashboard [Jenkins]" inurl:/job/
```
Exposed CouchDB Instances:
```
intitle:"Welcome to CouchDB" inurl:/_utils/
```
Open MongoDB Instances:
```
intitle:"MongoDB Status" "inMemory" inurl:/_stats/
```
Exposed Memcached Servers:
```
intitle:"Memcached Stats" inurl:/stats
```
Open NFS Exports:
```
intitle:"NFS status" inurl:/nfsstats.html
```
Open Elasticsearch Configurations:
```
intitle:"Elasticsearch Nodes Info" inurl:/_nodes
```
Exposed Grafana Dashboards:
```
intitle:"Grafana" inurl:/d/
```
Open Keycloak Login Pages:
```
intitle:"Keycloak" inurl:/auth/
```
Exposed Jenkins Scripts:
```
intitle:"Dashboard [Jenkins]" inurl:/script
```
Open SNMP Configuration Files:
```
intitle:"index of" "snmp.conf" OR "snmpd.conf" OR "snmpd.users" OR "snmpd.conf" OR "snmptt.ini"
```
Exposed Hadoop Cluster Information:
```
intitle:"Hadoop Administration" inurl:/dfshealth.html
```
Open Zabbix Monitoring Systems:
```
intitle:"Zabbix" intext:"Zabbix SIA"
```
Exposed Grafana Dashboards with Default Credentials:
```
intitle:"Grafana" intext:"login admin" intext:"password"
```
Open Docker Registry Servers:
```
intitle:"Index of" inurl:/v2/repositories/
```
Exposed Jupyter Notebook Configuration Files:
```
intitle:"Jupyter Notebook Configuration File" inurl:/tree
```
Open SonarQube Instances:
```
intitle:"SonarQube" inurl:/sonar
```
Exposed Mattermost Chat Servers:
```
intitle:"Mattermost" inurl:/login
```
Open Rsync Servers:
```
intitle:"rsync daemon" intext:"password file must not be other-readable"
```
Exposed OpenCart Admin Panels:
```
intitle:"OpenCart" inurl:/admin
```
Open phpBB Forums:
```
intext:"Powered by phpBB" inurl:/forum
```
Exposed DokuWiki Installations:
```
intitle:"DokuWiki Setup" inurl:/install.php
```
Open phpBB Configuration Files:
```
intitle:"phpBB" inurl:config.php intext:"Powered by phpBB" -site:phpbb.com
```
Exposed Nagios Servers:
```
intitle:"Nagios" intext:"Nagios Core"
```
Open Jenkins Pipeline Scripts:
```
intitle:"Jenkins Pipeline Syntax" inurl:/pipeline-syntax/
```
Exposed SNMP Configuration Files:
```
intitle:"Index of" intext:"snmpd.conf" OR intext:"snmpd.config" OR intext:"snmpd.cfg"
```
Open RDP Configuration Files:
```
intitle:"index of" "rdp.rdp"
```
Exposed Elastic Stack Kibana Dashboards:
```
intitle:"Kibana" intext:"Welcome to Kibana" inurl:/app/kibana
```
Open Jenkins Job Workspaces:
```
intitle:"Dashboard [Jenkins]" inurl:/job/*/ws/
```
