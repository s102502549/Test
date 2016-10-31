**Protype**  **C**** : **** UDP **** Client and Server ( ****UDP** 伺服端與客戶端雛形)

請寫一個UDP client，行為如下

1. 本程式執行起來先讓使用者輸入兩台電腦的IP address
例如 在 A 機器上執行後等待輸入，我們則輸入
     192.168.0.1
     192.168.0.2
2. 輸入完畢後，請假設此client維持了一個移動中的物件的座標(X,Y)。該座標由(0,0) 到 (100,100)。初始值為（0,0）。本UDP client 每隔2秒就將X座標與Y座標加1。也就是說座標固定由(X,Y)更新到（X＋1,Y＋1）。不過當X，Y的值到達100,100時，則將X，Y重新設定為（0,0），如此週而復始.
3. 每隔0.2秒，本UDP client 將最新的（X，Y）透過UDP message
&quot;X Y&quot;傳送給當初輸入的 server 端。

請寫一個UDP server 其行為如下

1. 本server 一執行後就進入無窮迴圈，等待UDP client 送來的messages。
2. 當收到message &quot;X Y&quot; 時，就列印出
（X，Y）
於螢幕上
3.
<img src="https://github.com/s102502549/Test/blob/master/Screenshot_2016-09-09-16-47-09.png">
