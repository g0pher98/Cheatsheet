# Cheatsheet about hacking
Cheetsheet for CTF and Penetration testing.

# INDEX
- [Table](#table)
	- [Ascii Code](#ascii-code)
	- [32bit System Call](#32bit-system-call)
	- [64bit System Call](#64bit-system-call)
- [Web](#web)
	- [SQL injection](#sql-injection)
	- [XSS](#xss)
	- [SSTI](#ssti)
	- [LFI & RFI](#lfi-rfi)
	- [XXE](#xxe)
	- [CSP Bypass](#csp-bypass)
- [Tools](#tools)
	- [RsaCtfTool](#rsactftool)
	


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
- Tech  
	https://www.hahwul.com/p/xxe-cheat-sheet.html

## CSP Bypass
- Tech  
	https://hahwul.com/2019/01/csp-bypass-technique-xss.html

# Tools
## RsaCtfTool
rsa 취약점 찾는 툴
- github  
	https://github.com/Ganapati/RsaCtfTool


# Table
## ascii code

| Dec |	Hex | Octal | Binary | Char | Description |
|---|---|---|---|---|---|
| 0 | 00 | 000 | 0000000 | NUL | null character |
| 1 | 01 | 001 | 0000001 | SOH | start of header |
| 2 | 02 | 002 | 0000010 | STX | start of text |
| 3 | 03 | 003 | 0000011 | ETX | end of text |
| 4 | 04 | 004 | 0000100 | EOT | end of transmission |
| 5 | 05 | 005 | 0000101 | ENQ | enquiry |
| 6 | 06 | 006 | 0000110 | ACK | acknowledge |
| 7 | 07 | 007 | 0000111 | BEL | bell (ring) |
| 8 | 08 | 010 | 0001000 | BS | backspace |
| 9 | 09 | 011 | 0001001 | HT | horizontal tab |
| 10 | 0A | 012 | 0001010 | LF | line feed |
| 11 | 0B | 013 | 0001011 | VT | vertical tab |
| 12 | 0C | 014 | 0001100 | FF | form feed |
| 13 | 0D | 015 | 0001101 | CR | carriage return |
| 14 | 0E | 016 | 0001110 | SO | shift out |
| 15 | 0F | 017 | 0001111 | SI | shift in |
| 16 | 10 | 020 | 0010000 | DLE | data link escape |
| 17 | 11 | 021 | 0010001 | DC1 | device control 1 |
| 18 | 12 | 022 | 0010010 | DC2 | device control 2 |
| 19 | 13 | 023 | 0010011 | DC3 | device control 3 |
| 20 | 14 | 024 | 0010100 | DC4 | device control 4 |
| 21 | 15 | 025 | 0010101 | NAK | negative acknowledge |
| 22 | 16 | 026 | 0010110 | SYN | synchronize |
| 23 | 17 | 027 | 0010111 | ETB | end transmission block |
| 24 | 18 | 030 | 0011000 | CAN | cancel |
| 25 | 19 | 031 | 0011001 | EM | end of medium |
| 26 | 1A | 032 | 0011010 | SUB | substitute |
| 27 | 1B | 033 | 0011011 | ESC | escape |
| 28 | 1C | 034 | 0011100 | FS | file separator |
| 29 | 1D | 035 | 0011101 | GS | group separator |
| 30 | 1E | 036 | 0011110 | RS | record separator |
| 31 | 1F | 037 | 0011111 | US | unit separator |
| 32 | 20 | 040 | 0100000 | space |  |
| 33 | 21 | 041 | 0100001 | ! | exclamation mark |
| 34 | 22 | 042 | 0100010 | " | quotation mark |
| 35 | 23 | 043 | 0100011 | # | number sign |
| 36 | 24 | 044 | 0100100 | $ | dollar sign |
| 37 | 25 | 045 | 0100101 | % | percent sign |
| 38 | 26 | 046 | 0100110 | & | ampersand |
| 39 | 27 | 047 | 0100111 | ' | apostrophe |
| 40 | 28 | 050 | 0101000 | ( | left parenthesis |
| 41 | 29 | 051 | 0101001 | ) | right parenthesis |
| 42 | 2A | 052 | 0101010 | * | asterisk |
| 43 | 2B | 053 | 0101011 | + | plus sign |
| 44 | 2C | 054 | 0101100 | , | comma |
| 45 | 2D | 055 | 0101101 | - | hyphen |
| 46 | 2E | 056 | 0101110 | . | period |
| 47 | 2F | 057 | 0101111 | / | slash |
| 48 | 30 | 060 | 0110000 | 0 | digit 0 |
| 49 | 31 | 061 | 0110001 | 1 | digit 1 |
| 50 | 32 | 062 | 0110010 | 2 | digit 2 |
| 51 | 33 | 063 | 0110011 | 3 | digit 3 |
| 52 | 34 | 064 | 0110100 | 4 | digit 4 |
| 53 | 35 | 065 | 0110101 | 5 | digit 5 |
| 54 | 36 | 066 | 0110110 | 6 | digit 6 |
| 55 | 37 | 067 | 0110111 | 7 | digit 7 |
| 56 | 38 | 070 | 0111000 | 8 | digit 8 |
| 57 | 39 | 071 | 0111001 | 9 | digit 9 |
| 58 | 3A | 072 | 0111010 | : | colon |
| 59 | 3B | 073 | 0111011 | ; | semicolon |
| 60 | 3C | 074 | 0111100 | < | less than |
| 61 | 3D | 075 | 0111101 | = | equals to |
| 62 | 3E | 076 | 0111110 | > | greater than |
| 63 | 3F | 077 | 0111111 | ? | question mark |
| 64 | 40 | 100 | 1000000 | @ | at sign |
| 65 | 41 | 101 | 1000001 | A | uppercase A |
| 66 | 42 | 102 | 1000010 | B | uppercase B |
| 67 | 43 | 103 | 1000011 | C | uppercase C |
| 68 | 44 | 104 | 1000100 | D | uppercase D |
| 69 | 45 | 105 | 1000101 | E | uppercase E |
| 70 | 46 | 106 | 1000110 | F | uppercase F |
| 71 | 47 | 107 | 1000111 | G | uppercase G |
| 72 | 48 | 110 | 1001000 | H | uppercase H |
| 73 | 49 | 111 | 1001001 | I | uppercase I |
| 74 | 4A | 112 | 1001010 | J | uppercase J |
| 75 | 4B | 113 | 1001011 | K | uppercase K |
| 76 | 4C | 114 | 1001100 | L | uppercase L |
| 77 | 4D | 115 | 1001101 | M | uppercase M |
| 78 | 4E | 116 | 1001110 | N | uppercase N |
| 79 | 4F | 117 | 1001111 | O | uppercase O |
| 80 | 50 | 120 | 1010000 | P | uppercase P |
| 81 | 51 | 121 | 1010001 | Q | uppercase Q |
| 82 | 52 | 122 | 1010010 | R | uppercase R |
| 83 | 53 | 123 | 1010011 | S | uppercase S |
| 84 | 54 | 124 | 1010100 | T | uppercase T |
| 85 | 55 | 125 | 1010101 | U | uppercase U |
| 86 | 56 | 126 | 1010110 | V | uppercase V |
| 87 | 57 | 127 | 1010111 | W | uppercase W |
| 88 | 58 | 130 | 1011000 | X | uppercase X |
| 89 | 59 | 131 | 1011001 | Y | uppercase Y |
| 90 | 5A | 132 | 1011010 | Z | uppercase Z |
| 91 | 5B | 133 | 1011011 | \[ | left square bracket |
| 92 | 5C | 134 | 1011100 | \ | backslash |
| 93 | 5D | 135 | 1011101 | ] | right square bracket |
| 94 | 5E | 136 | 1011110 | ^ | caret |
| 95 | 5F | 137 | 1011111 | _ | underscore |
| 96 | 60 | 140 | 1100000 | \` | backtick |
| 97 | 61 | 141 | 1100001 | a | lowercase a |
| 98 | 62 | 142 | 1100010 | b | lowercase b |
| 99 | 63 | 143 | 1100011 | c | lowercase c |
| 100 | 64 | 144 | 1100100 | d | lowercase d |
| 101 | 65 | 145 | 1100101 | e | lowercase e |
| 102 | 66 | 146 | 1100110 | f | lowercase f |
| 103 | 67 | 147 | 1100111 | g | lowercase g |
| 104 | 68 | 150 | 1101000 | h | lowercase h |
| 105 | 69 | 151 | 1101001 | i | lowercase i |
| 106 | 6A | 152 | 1101010 | j | lowercase j |
| 107 | 6B | 153 | 1101011 | k | lowercase k |
| 108 | 6C | 154 | 1101100 | l | lowercase l |
| 109 | 6D | 155 | 1101101 | m | lowercase m |
| 110 | 6E | 156 | 1101110 | n | lowercase n |
| 111 | 6F | 157 | 1101111 | o | lowercase o |
| 112 | 70 | 160 | 1110000 | p | lowercase p |
| 113 | 71 | 161 | 1110001 | q | lowercase q |
| 114 | 72 | 162 | 1110010 | r | lowercase r |
| 115 | 73 | 163 | 1110011 | s | lowercase s |
| 116 | 74 | 164 | 1110100 | t | lowercase t |
| 117 | 75 | 165 | 1110101 | u | lowercase u |
| 118 | 76 | 166 | 1110110 | v | lowercase v |
| 119 | 77 | 167 | 1110111 | w | lowercase w |
| 120 | 78 | 170 | 1111000 | x | lowercase x |
| 121 | 79 | 171 | 1111001 | y | lowercase y |
| 122 | 7A | 172 | 1111010 | z | lowercase z |
| 123 | 7B | 173 | 1111011 | { | left curly brace |
| 124 | 7C | 174 | 1111100 | \| | vertical bar |
| 125 | 7D | 175 | 1111101 | } | right curly brace |
| 126 | 7E | 176 | 1111110 | ~ | tilde |
| 127 | 7F | 177 | 1111111 | DEL | delete (rubout) |

https://www.asciitable.xyz/
## 32bit system call

|name|eax|ebx|ecx|edx|esi|edi|
|:---|:---|:---|:---|:---|:---|:---|
|sys_exit|0x01|error_code|
|sys_fork|0x02|pt_regs|
|sys_read|0x03|fd|buf|count|
|sys_write|0x04|fd|buf|count|
|sys_open|0x05|filename|flags|mode|
|sys_close|0x06|fd|
|sys_execve|0x0b|filename|argv|envp|

http://syscalls.kernelgrok.com/
## 64bit system call

|name|eax|ebx|ecx|edx|esi|edi|
|:---|:---|:---|:---|:---|:---|:---|
|sys_read|0|fd|buf|count|
|sys_write|1|fd|buf|count|
|sys_open|2|filename|flags|mode|
|sys_close|3|fd|
|sys_execve|59|filename|argv|envp|

https://crasy.tistory.com/75



