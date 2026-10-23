Information disclosure vulnerability in Intern Record System In PHP With Source Code (code-projects.org)

VENDOR : CODE-PROJECTS.ORG

Project: Intern Record System In PHP With Source Code (https://code-projects.org/intern-record-system-in-php-with-source-code/)

Description: Found information Disclosure in this project where anyone can traverse through the /department.sql and the file gets installed on the system leading to leak of sensitive information.

Steps to reproduce:

1.  setup the project and go through https://localhost/intern
![POC(images/db_1.png)]

2. go to /department.sql and sql file will be downloaded.
![POC(images/db_2.png)]

3. Open it with any editor tool and sensitive info can be viewed.
![POC(images/db_3.png)]

Impact:

Leak of sensitive information and exposure of data.

Recommendation: restrict the path through /department.sql file 
