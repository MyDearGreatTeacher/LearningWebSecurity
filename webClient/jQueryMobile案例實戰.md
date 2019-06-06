
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
      var msg = new Array("Docker是一個開放原始碼軟體專案，讓應用程式部署在軟體貨櫃下的工作可以自動化進行", 
	    "Dockers是有能力打包應用程式及其虛擬容器，可以在任何Linux伺服器上執行的依賴性工具", 
		"Docker利用Linux核心中的資源分離機制，例如cgroups，以及Linux核心命名空間（namespaces），來建立獨立的容器（containers）"); 
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
//小測驗:: data-position="fixed"
      <div data-role="header" data-position="fixed">  
 	    <h1>T-shirt 王Docker</h1>
      </div>
      <div data-role="content">	    
		<img src="piece.jpg" width="100%"> 
	    <a href="#story" data-rel="dialog" data-role="button" data-icon="arrow-r">Docker介紹</a>
		<a href="#role" data-role="button" data-icon="arrow-r">Docker功能介紹</a>
		<a href="https://www.docker.com/" data-rel="external" data-role="button" data-icon="arrow-r">Docker官方網站</a>
	  </div>
//表尾===使用data-role="footer"  
      <div data-role="footer" data-position="fixed">
	    <h4>&copy;快樂學Docker</h4>
	  </div>
    </div>
    
    
 //定義story	
	<div data-role="page" id="story">
	  <div data-role="header">
	    <h1>Docker介紹</h1>	            
      </div>
      <div data-role="content">
        <p>Docker是一個開放原始碼軟體專案，讓應用程式部署在軟體貨櫃下的工作可以自動化進行，藉此在Linux作業系統上，
		提供一個額外的軟體抽象層，以及作業系統層虛擬化的自動管理機制[1]。

Docker利用Linux核心中的資源分離機制，例如cgroups，以及Linux核心命名空間（namespaces），來建立獨立的容器（containers）。這可以在單一Linux實體下運作，避免啟動一個虛擬機器造成的額外負擔[2]。Linux核心對命名空間的支援完全隔離了工作環境中應用程式的視野，包括行程樹、網路、用戶ID與掛載檔案系統，而核心的cgroup提供資源隔離，包括CPU、記憶體、block I/O與網路。從0.9版本起，Dockers在使用抽象虛擬是經由libvirt的LXC與systemd - nspawn提供介面的基礎上，開始包括libcontainer函式庫做為以自己的方式開始直接使用由Linux核心提供的虛擬化的設施，

依據行業分析公司「451研究」：「Dockers是有能力打包應用程式及其虛擬容器，可以在任何Linux伺服器上執行的依賴性工具，這有助於實現靈活性和可攜式性，應用程式在任何地方都可以執行，無論是公有雲、私有雲、單機等。</p>
      </div>
	</div>


//定義role
	<div data-role="page" id="role">
	  <div data-role="header">
	    <h1>Docker介紹</h1>	            
      </div>
	  <div data-role="content">
	    <img id="roleimg" src="piece1.jpg" width="100%">
		<p id="rolemsg">Docker利用Linux核心中的資源分離機制。</p>
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
