#

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

###
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
