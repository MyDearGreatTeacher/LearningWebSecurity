
# 登入的畫面 index.html

```
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
	<title>T-shirt 王的行動網站</title>
	<link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css" />
    <script src="http://code.jquery.com/jquery-2.2.3.min.js"></script>
    <script src="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>    
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<script>
	  var i = 0;
      var img = new Array("piece1.jpg", "piece2.jpg", "piece3.jpg");
      var msg = new Array("「喬巴」－夢想成為能治百病的神醫。", 
	    "「索隆」－夢想成為世界第一的劍士。", 
		"「佛朗基 」－傳說中的船匠湯姆的弟子，打造了千陽號。"); 
	  function prev(){
	    i--; 
	    if (i < 0) {i = 2;}
	    $("#roleimg").attr("src", img[i]);		
		$("#rolemsg").text(msg[i]);
      }
	  function next(){
	    i++; 
	    if (i > 2) {i = 0;}
	    $("#roleimg").attr("src", img[i]);		
		$("#rolemsg").text(msg[i]);
      }
	</script>
  </head>
  <body>  
  //整個網頁==使用data-role="page"   網頁id="home"
    <div data-role="page" id="home">
   //表頭===使用data-role="header"
      <div data-role="header" data-position="fixed">  
 	    <h1>T-shirt 王</h1>
      </div>
   //內容==使用  data-role="content"
      <div data-role="content">	    
		<img src="piece.jpg" width="100%"> 
	    <a href="#story" data-rel="dialog" data-role="button" data-icon="arrow-r">故事介紹</a>
		<a href="#role" data-role="button" data-icon="arrow-r">角色介紹</a>
		<a href="http://www.ttv.com.tw/drama/2005/cartoon/onepeace/01-story.htm" data-rel="external" data-role="button" data-icon="arrow-r">航海王官方網站</a>
	  </div>	  
   //表頭===使用data-role="header"	  
   //小測驗:: data-position="fixed"
      <div data-role="footer" data-position="fixed">
	    <h4>&copy;快樂Docker</h4>
	  </div>
    </div>
 
 //定義story
     <div data-role="page" id="story">
	  <div data-role="header">
	    <h1>Docker介紹</h1>	            
      </div>
      <div data-role="content">
        <p>海賊王Docker遺留下一個被稱為ONEPIECE的神秘寶藏，
        而主角「LUFU Docker」找了海盜剋星「So long Docker」、女賊「na mei Docker」、
        可愛馴鹿「chifu Docker」等幾位夥伴要一起尋找傳說中的寶藏。</p>
      </div>
	</div>
 //定義role	
	<div data-role="page" id="role">
	  <div data-role="header">
	    <h1>人物介紹</h1>	            
      </div>
      //第一個腳色
	  <div data-role="content">
	    <img id="roleimg" src="piece1.jpg" width="100%">
		<p id="rolemsg">「chou ba dcoker」－夢想成為能治百病的神醫。</p>
	  </div>
	  <div data-role="footer" data-position="fixed">
	    <div data-role="navbar">
	      <ul>
            <li><a href="#home" class="ui-btn-active ui-state-persist">回首頁</a></li>
            <li><a href="javascript:prev();">上一個</a></li>
            <li><a href="javascript:next();">下一個</a></li>
          </ul>
	    </div>  
      </div>
	</div>	
  </body>
</html>
```
