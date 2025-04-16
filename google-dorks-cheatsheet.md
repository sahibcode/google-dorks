Google Dorks Cheatsheet

This cheatsheet provides 50 categorized Google dorks for cybersecurity professionals. These queries help identify vulnerabilities, exposed data, and misconfigurations. Use responsibly and ethically, only on systems you have permission to test.



Exposed Databases







Dork



Description





inurl:phpmyadmin intitle:"phpMyAdmin" -inurl:demo



Finds exposed phpMyAdmin interfaces, excluding demo sites.





filetype:sql intext:"insert into" "password"



Finds SQL dump files containing password data.





intitle:"index of" "database.sql"



Finds directories exposing database backup files.





inurl:/_utils/ intitle:"CouchDB"



Finds exposed CouchDB interfaces.





intext:"mongodb://" filetype:config



Finds config files with MongoDB connection strings.



Vulnerable Web Applications







Dork



Description





inurl:"id=" intitle:"error" "sql syntax"



Finds pages with SQL errors, hinting at SQL injection risks.





inurl:admin intitle:"login" -inurl:wp-admin



Finds admin login pages, excluding WordPress.





intext:"warning: mysql_connect()" "invalid" "password"



Finds MySQL errors revealing database credentials.





inurl:login.php intitle:"login" "admin"



Finds generic admin login pages.





intext:"phpinfo()" filetype:php



Finds phpinfo() pages exposing server details.



Sensitive Directories







Dork



Description





intitle:"index of" "parent directory"



Finds open directories with parent listings.





inurl:.git intitle:"index of" "config"



Finds exposed Git directories with config files.





filetype:log intext:"password"



Finds log files containing password information.





intitle:"index of" "backup"



Finds directories with backup files.





inurl:/wp-content/uploads/ intitle:"index of"



Finds exposed WordPress upload directories.



WordPress







Dork



Description





inurl:wp-content intitle:"index of"



Finds exposed WordPress content directories.





intext:"powered by wordpress" inurl:wp-login.php



Finds WordPress login pages.





inurl:wp-admin intitle:"login"



Finds WordPress admin login pages.





filetype:php intext:"wp_"



Finds WordPress-related PHP files (e.g., plugins/themes).





inurl:wp-json intitle:"index of"



Finds exposed WordPress REST API endpoints.



Cloud Services







Dork



Description





site:s3.amazonaws.com intitle:"index of"



Finds open AWS S3 buckets.





inurl:blob.core.windows.net intitle:"index of"



Finds open Azure Blob Storage containers.





site:storage.googleapis.com intitle:"index of"



Finds open Google Cloud Storage buckets.





intext:"aws_access_key_id" filetype:txt



Finds text files with AWS access keys.





inurl:/_snapshot/ intitle:"ElasticSearch"



Finds exposed ElasticSearch snapshot directories.



Exposed Credentials







Dork



Description





intext:"api_key" filetype:txt



Finds text files containing API keys.





intitle:"index of" "id_rsa"



Finds directories exposing SSH private keys.





intext:"password" filetype:env



Finds environment files with passwords.





inurl:/config/ intitle:"index of" "database"



Finds config directories with database credentials.





intext:"private_key" filetype:pem



Finds PEM files containing private keys.



IoT Devices







Dork



Description





inurl:/login.htm intitle:"login" "IoT"



Finds login pages for IoT devices.





intext:"default password" "IoT"



Finds pages mentioning default IoT passwords.





inurl:/cgi-bin/ intitle:"IoT"



Finds vulnerable CGI scripts on IoT devices.





intitle:"IoT" intext:"admin" "password"



Finds pages with IoT admin credentials.





inurl:/device.rsp intitle:"IoT"



Finds IoT device response pages.



Exposed Webcams







Dork



Description





inurl:/axis-cgi/mjpg



Finds Axis webcams with MJPG streams.





intitle:"Live View / - AXIS"



Finds live views from Axis webcams.





inurl:/view/viewer_index.shtml



Finds generic webcam viewer pages.





intitle:"webcamXP" inurl:8080



Finds webcams using webcamXP software.





inurl:/video.cgi intitle:"IP Camera"



Finds IP cameras with video CGI scripts.



Exposed Documents







Dork



Description





filetype:pdf intext:"confidential"



Finds PDFs marked as confidential.





filetype:xls intext:"username" "password"



Finds Excel files with usernames and passwords.





filetype:doc intext:"sensitive"



Finds Word docs with sensitive information.





filetype:txt intext:"credit card"



Finds text files mentioning credit card info.





filetype:csv intext:"email" "password"



Finds CSV files with email and password data.
