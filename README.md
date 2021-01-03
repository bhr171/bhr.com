
<!DOCTYPE html>
<html>
<head>
<title> I Love You </title>
<link rel="shortcut icon" type="image/gif" href="http://www.goodlightscraps.com/content/i_love_you/i_love_u_25.gif" />
<meta name="Author" content="SXT0 @sams_sitorus">
<meta http-equiv="imagetoolbar" content="no">
<style type="text/css">
html {
overflow: hidden;
}
body {
position: absolute;
margin: 0px;
padding: 0px;
background: #000000;
width: 100%;
height: 100%;
}
#container {
position: absolute;
background: URL("http://t1.gstatic.com/images?q=tbn:ANd9GcRoFjbUHdzs7hJEojGCi9r5vJwzNiDKbMf8N_Cz4zvp0dIGAPRo");
left: 50%;
top: 50%;
width: 640px;
height: 360px;
margin-left: -320px;
margin-top: -180px;
overflow: hidden;
font-size: 1em;
box-shadow: 10px 10px 5px #999;
}
#inkp1 {
position: absolute;
top: 55px;
left: 10px;
}
#inkp2 {
position: absolute;
top: 55px;
left: 10px;
}
#sound {
position: absolute;
right: 15px;
bottom: 15px;
cursor: pointer;
}
#typewriter {
position: absolute;
width: 100%;
height: 100%;
overflow: hidden;
}
#resources {
display:none;
}
</style>
<script type="text/javascript">
// ===============================================
// ---- QUILL TYPEWRITER ---
// Script by sam_xto

// Edited script - October'13
// ===============================================
// http://www.samuelscouter.blogspot.com
// ===============================================

"use strict";

(function () {
var t = "", p = 0, c = "", cc = "", mm = "<span>";
var cl = 0, mr = "<br><br>", context, inkFreq, spdInk, mute = false;
var $ = function (id) {
return document.getElementById(id);
}
var init = function (data) {
context = $(data.context);
inkFreq = data.inkFreq;
spdInk = data.spdInk;
t = $(data.text).innerHTML;
c = " <img src='" + $("cursor").src + "' style='position:absolute'>" + mr;
run();
$("write").play();
$("sound").addEventListener('click', function () {
mute = !mute;
if (mute) {
$("sound").style.opacity = "0.3";
$("music").pause();
} else {
$("sound").style.opacity = "1";
$("music").play();
}
}, false);
}
var run = function () {
var m = t.charAt(p);
var tmp = 32;
if (m == "") cc = mr;
else if (m == "|") {
m = "";
mm = mm.substring(0, mm.length-1);
tmp = 64;
} else if (m == "<") {
var av = t.indexOf(">", p);
m = t.substring(p, av + 1);
p = av;
} else if (m == "&") {
var av = t.indexOf(";", p);
m = t.substring(p, av + 1);
p = av;
} else if (m == ".") tmp = 250;
else if (m == ",") tmp = 100;
else if (m == " ") tmp = 32;
else if (p > 10) cc = c;
if (m == " ") {
cl += spdInk;
m = '</span><span style="color:RGB(' + (cl) + ',' + (cl) + ',' + (cl) + ')">' + m;
if (cl < 40 && Math.random() > inkFreq)
m += ' <img src = "' + $("ink").src + '" align = "absmiddle"> ';
}
if ($("inkp2").style.visibility == "visible") {
cc = c;
$("inkp2").style.visibility = "hidden";
$("reload").pause();
$("write").play();
m = '</span><span style="color:RGB(0,0,0)">' + m;
}
if (cl > 180) {
cl = 0;
$("inkp2").style.visibility = "visible";
$("reload").play();
$("write").pause();
tmp = 1000;
cc = mr;
}
mm += m;
if (p == t.length - 1) cc = mr;
context.innerHTML = mm + cc;
context.scrollTop = 100000;
p++;
if (p < t.length) setTimeout(run, 32 + tmp);
else {
$("reload").pause();
$("write").pause();
context.style.overflow = "auto";
}
}
return {
load : function (data) {
window.addEventListener('load', function () {
setTimeout(function () {
init(data);
}, 900);
}, false);
}
}
})().load({
text: "text",
context: "typewriter",
inkFreq: 0.7,
spdInk: 12
});
</script>
</style>

</head>
<br>

<img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcS0Ejcxxl8P6O5911voZzGw20r9xNTCGteo15knrp5C0PIk6zbOvw" align="right">

<img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcS0Ejcxxl8P6O5911voZzGw20r9xNTCGteo15knrp5C0PIk6zbOvw" align="left">

<body oncontextmenu='return false;' onkeydown='return false;' onmousedown='return false;'><script type="text/javascript">
    function setAttributeOnload(object, attribute, val) {
      if(window.addEventListener) {
        window.addEventListener('load',
          function(){ object[attribute] = val; }, false);
      } else {
        window.attachEvent('onload', function(){ object[attribute] = val; });
      }
    }
  </script>
<div id="navbar-iframe-container"></div>
<script type="text/javascript" src="https://apis.google.com/js/plusone.js"></script>

<div id="container">
<div id="typewriter">
</div>
<img id="inkp1" src="http://www.casperia.com/Esempio%20completo/encrierplume.gif" alt="">
<img id="inkp2" src="http://www.casperia.com/Esempio%20completo/encrierplume.gif" alt="">
<img id="sound" src="http://www.drac-101code.com/speaker_silent_32.png" alt="">
</div>
<div id="resources">
<img id="ink" src="http://www.drac-101code.com/tache.jpg" alt="">
<img id="cursor" src="http://www.verkehrsverein-messinghausen.de/images/plumeBouge.gif" alt="">
<div id="text">
<div style="margin: 1em;margin-left:100px;font-style:italic;font-family:arial, Comic Sans MS;font-size:1em;">

Biarlah aku mengagumi<br>
Biarkan aku memandangmu<br>
Biarkan aku menikmati indahnya senyummu<br>
Walaupun itu semua ku lakukan dari kejauhan<br>
Yang mungkin takkan pernah kau sadari.<br>
Aku lakukan hal itu,<br>
Bukan semata-mata karna ku malu.<br>
Tapi,<br>
Aku takut jika nanti aku tidak bisa berbicara<br>
Aku juga takut tidak bisa membuatmu tertawa<br>
Karena aku juga tidak romantis<br>
Mungkin......<br>
Aku memang bukan orang yang baik untukmu.<br>
Namun,<br>
Atas semua itu,<br>
Aku menyayangimu<br>
Aku  takut kehilanganmu<br>
Ingatlah suatu hal,<br>
Aku juga sangat mencintaimu.<br>
<br>
I <span style="color:red; font-family:arial, comic sans ms;">Love</span> You<br>

</div>
</div>
</div>
<audio id="write" preload="auto" loop>
<source src="http://www.dhteumeuleu.com/sound/plume.mp3" type="audio/mpeg">
<source src="http://www.dhteumeuleu.com/sound/plume.ogg" type="audio/ogg">
</audio>

<audio id="reload" preload="auto" loop>
<source src="http://www.dhteumeuleu.com/sound/pop.mp3" type="audio/mpeg">
<source src="http://www.dhteumeuleu.com/sound/pop.ogg" type="audio/ogg">
</audio>

<source src="http://www.dhteumeuleu.com//sound/Albeniz_Asturias_converted.ogg" type="audio/ogg">
</audio>
<img style="visibility:hidden;width:0px;height:0px;" border=0 width=0 height=0 src="http://c.gigcount.com/wildfire/IMP/CXNID=2000002.0NXC/bT*xJmx*PTEzNDgzOTQyNzcxMjUmcHQ9MTM*ODM5NDMzNTA2MiZwPTEzNzkyMSZkPSZnPTEmbz1lNDM1NjMyNTA1ZDE*ODhlOWVh/NjBmZmUyOTcyYmVmZiZvZj*w.gif" /> <center>
<embed width="5" height="5" flashvars="playerID=1&bg=0xffffff&leftbg=0xCA4536&lefticon=0xffffff&rightbg=0xCA4536&rightbghover=0x999999&righticon=0xffffff&righticonhover=0xffffff&text=0xCA4536&slider=0x303030&track=0xFFFFFF&border=0x666666&loader=0xC52C24&autostart=yes&loop=yes&soundFile=http://videokeman.com/dload/flvs/v17/Secondhand_Serenade-Your_Call.doc" wmode="transparent" src="http://videokeman.com/music/videokemanplay.swf"></embed>
<br /><small><a href="http://www.musicdumper.com/" target="_blank"></a></small></center>
<script type="text/javascript">
//Define first typing example:
new TypingText(document.getElementById("example1"));
//Define second typing example (use "slashing" cursor at the end):
new TypingText(document.getElementById("example2"), 50, function(i){
var ar = new Array("_"," ","_"," "," "); return " " + ar[i.length %
ar.length]; });
//Type out examples:
TypingText.runAll();
</script>
<script language="JavaScript1.2">
function disableselect(e){
return false
}
function reEnable(){
return true
}
document.onselectstart=new Function ("return false")
if (window.sidebar){
document.onmousedown=disableselect
document.onclick=reEnable
}
</script>

    <script language=JavaScript>
    <!--
   //Disable right click script III- By SXT0
   //For full source code, visit http://www.samuelscouter.blogspot.com
   var message="";
   ///////////////////////////////////
   function clickIE() {if (document.all) {(message);return false;}}
   function clickNS(e) {if
   (document.layers||(document.getElementById&&!document.all)) {
   if (e.which==2||e.which==3) {(message);return false;}}}
   if (document.layers)
   {document.captureEvents(Event.MOUSEDOWN)
   ;document.onmousedown=clickNS;}
   else{document.onmouseup=clickNS;document.oncontextmenu=clickIE;}
   document.oncontextmenu=new Function("return false")
   // -->
    </script>
        <script type="text/javascript" src="//www.blogger.com/static/v1/common/js/1447355603-csitail.js"></script>
 Ket >>
