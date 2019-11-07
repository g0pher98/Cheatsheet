# Cheatsheet about hacking
Cheetsheet for CTF and Penetration testing.

# Web
## SQL injection
or가 필터링 되는 경우가 있는데, oorr로 우회할 수 없다면 information schema를 사용하지 않는 문제다. information에 or가 포함되어있기 때문. 이 경우에는 테이블 내부에 플래그가 있을 확률이 높은데, or를 안쓰고 공격 쿼리를 완성해야한다. 예를들어 `1'*1 limit 0,1#`로 0부터 탐색하거나 like 문의 경우 `' limit 0,1#`로 탐색할 수 있다. 만약 컬럼명을 알고있거나, 추측할 수 있다면 `1'*1 and id='abc`와 같은 형태로 blind sqli로 접근해볼 수 있다. 간단하게 먹히는 문제는 sqlmap으로 충분히 풀이가 가능하다.
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
보통 게시판이나 쪽지 형태로 문제가 구성된다. 목표는 xss를 통해 관리자의 세션을 탈취해서 관리자의 글을 읽거나 해당 세션으로 로그인하게 되면 홈페이지에 플래그가 있는 경우가 있다. 문제는 xss 스크립트를 작성하는 부분인데 보통 csp나 필터링이 걸려있다. 개발자도구의 네트워크 탭에서 csp를 확인할 수 있고, 아래 csp bypass 링크를 참고해서 잘 우회해야한다. 필터링은 xss 링크를 참고해서 공격하면 된다. 스크립트는 해당 글이 업로드 되고 view 할때 `ctrl + u`를 눌러서 소스코드를 보고 스크립트가 안먹히는 원인인 태그를 찾아야 한다 (`<pre>`나 `<code>`) 이런 태그들을 하나씩 닫아주고, script 태그가 실행될 수 있도록 하면 된다.
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
요즘 url을 통해 장난칠 수 있는 문제가 많이 나오는데, 샵(#)이나 물음표(?)를 통해 마치 sqli의 주석처럼 사용할 수 있다. 예를들면 "http://ctf.com/injection/../../../../../../../etc/passwd#/anythingsalt"가 될 수 있다.
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


