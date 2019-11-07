# Cheatsheet about hacking
Cheetsheet for CTF and Penetration testing.

# Web
## SQL injection
### Tech
- SQL tech  
	https://www.netsparker.com/blog/web-security/sql-injection-cheat-sheet/  
- MySQL injection  
	http://pentestmonkey.net/cheat-sheet/sql-injection/mysql-sql-injection-cheat-sheet  
- MSSQL injection  
	http://pentestmonkey.net/cheat-sheet/sql-injection/mssql-sql-injection-cheat-sheet  
- Oracle SQL injection  
	http://pentestmonkey.net/cheat-sheet/sql-injection/oracle-sql-injection-cheat-sheet  
	
### Functions
- MySQL functions  
	https://www.techonthenet.com/mysql/functions/index.php
- MariaDB functions  
	https://www.techonthenet.com/mariadb/functions/index.php
- PostgreSQL functions  
	https://www.techonthenet.com/postgresql/functions/index.php  
- SQLite functions  
	https://www.techonthenet.com/sqlite/functions/index.php
- Oracle SQL functions  
	https://www.techonthenet.com/oracle/functions/index.php


## XSS
- Tech  
	https://www.hahwul.com/2016/06/web-hacking-anti-xss-filter-evasion-of.html
- Payloads  
	https://gbhackers.com/top-500-important-xss-cheat-sheet/  
	https://gist.github.com/kurobeats/9a613c9ab68914312cbb415134795b45

## SSTI
인풋값에 `{{3*3}}`(python) 이나 `${{3*3}}`(Java) 등과 같은 형식의 인젝션이 먹힐 때
- 플랫폼 별 SSTI Tech  
	https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Server%20Side%20Template%20Injection
- Python SSTI Tech (Flask, Django ...)  
	https://www.lanmaster53.com/2016/03/11/exploring-ssti-flask-jinja2-part-2/
- Java SSTI Tech (Spring ...)  
	https://hawkinsecurity.com/2017/12/13/rce-via-spring-engine-ssti/

## LFI & RFI
- Tech  
	https://securitycode.tistory.com/49

## XXE
XML을 주입할 수 있을 때 가능한 공격으로, LFI & RFI로 공격이 이어질 수 있다.
- Tech  
	https://www.hahwul.com/p/xxe-cheat-sheet.html

## CSP Bypass
응답 헤더에서 csp를 확인할 수 있다. 걸려있으면 우회하는 문제일 확률이 높다.
- Tech  
	https://hahwul.com/2019/01/csp-bypass-technique-xss.html

# Tools
## RsaCtfTool
rsa 취약점 찾는 툴
- github  
	https://github.com/Ganapati/RsaCtfTool


