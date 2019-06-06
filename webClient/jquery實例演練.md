# jQuery 語法
```
jQuery 語法是通過選取 HTML 元素，並對選取的元素執行某些操作。

基礎語法： $(selector).action()

美元符號定義 jQuery
選擇符（selector）"查詢"和"查找" HTML 元素
jQuery 的 action() 執行對元素的操作

實例:
$(this).hide() - 隱藏當前元素
$("p").hide() - 隱藏所有 <p> 元素
$("p.test").hide() - 隱藏所有 class="test" 的 <p> 元素
$("#test").hide() - 隱藏所有 id="test" 的元素
```

# 範例一:
```

```

```
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<script src="https://cdn.staticfile.org/jquery/1.10.2/jquery.min.js">
</script>
<script>
$(document).ready(function(){
  $("button").click(function(){
    $("#div1").fadeIn();
    $("#div2").fadeIn("slow");
    $("#div3").fadeIn(3000);
  });
});
</script>
</head>

<body>
<p>實例演練 fadeIn() 使用了不同參數的效果。</p>
<button>點擊淡入 div 元素。</button>
<br><br>
<div id="div1" style="width:80px;height:80px;display:none;background-color:red;"></div><br>
<div id="div2" style="width:80px;height:80px;display:none;background-color:green;"></div><br>
<div id="div3" style="width:80px;height:80px;display:none;background-color:blue;"></div>

</body>
</html>
```
### 使用CDN
```
<script src="https://cdn.staticfile.org/jquery/1.10.2/jquery.min.js">

```

# 範例二:

```
<html>
<head>
<script type="text/javascript" src="/jquery/jquery.js"></script>
<script type="text/javascript">
$(document).ready(function(){
  $(".btn1").click(function(){
  $("p").fadeOut()
  });
  $(".btn2").click(function(){
  $("p").fadeIn();
  });
});
</script>
</head>
<body>
<p>This is a paragraph.</p>
<button class="btn1">Hide</button>
<button class="btn2">Show</button>
</body>
</html>
```

# 範例三:

```
資料來雲:http://www.w3school.com.cn/jquery/jquery_animate.asp
```
```
<!DOCTYPE html>
<html>
<head>
<script src="/jquery/jquery-1.11.1.min.js"></script>
<script> 
$(document).ready(function(){
  $("button").click(function(){
    var div=$("div");  
    div.animate({left:'100px'},"slow");
    div.animate({fontSize:'3em'},"slow");
  });
});
</script> 
</head>

<body>

<button>開始動畫</button>
<p>預設情況下，所有 HTML 元素的位置都是靜態的，並且無法移動。如需對位置進行操作，記得首先把元素的 CSS position 屬性設置為 relative、fixed 或 absolute。</p>
<div style="background:#98bf21;height:100px;width:200px;position:absolute;">HELLO</div>

</body>
</html>
```
