###
有關Bootstrap的說明ㄝ下列何者為非?
```
Bootstrap 是全球最受歡迎的前端元件庫，用於開發回應式佈局、移動設備優先的 WEB 專案。

Bootstrap4 目前是 Bootstrap 的最新版本，是一套用於 HTML、CSS 和 JS 開發的開源工具集。
利用提供的 Sass 變數和大量 mixin、回應式柵格系統、可擴展的預製元件、
基於 jQuery 的強大的外掛程式系統，
能夠快速為你的想法開發出原型或者構建整個 app 。
```

```
<!DOCTYPE html>
<html>
<head>
  <title>Bootstrap實例</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://cdn.staticfile.org/twitter-bootstrap/4.1.0/css/bootstrap.min.css">

/*  使用CDN */
  <script src="https://cdn.staticfile.org/jquery/3.2.1/jquery.min.js"></script>
  <script src="https://cdn.staticfile.org/popper.js/1.12.5/umd/popper.min.js"></script>
  <script src="https://cdn.staticfile.org/twitter-bootstrap/4.1.0/js/bootstrap.min.js"></script>

</head>
<body>

//第一個橫幅
<div class="jumbotron text-center">
  <h1>我的第一個 Bootstrap 頁面</h1>
  <p>重置流覽器大小查看效果!</p> 
</div>

//第二個:容器container
<div class="container">
  <div class="row">
    <div class="col-sm-4">
      <h3>第一列</h3>
      <p>b Bootstrap教程</p>
      <p>學的不僅是技術，更是夢想！！！</p>
    </div>
    <div class="col-sm-4">
      <h3>第二列</h3>
      <p> Bootstrap教程..</p>
      <p>學的不僅是技術，更是夢想！！！</p>
    </div>
    <div class="col-sm-4">
      <h3>第三列</h3> 
      <p> Bootstrap教程..</p>
      <p>學的不僅是技術，更是夢想！！！夢想一定要成真</p>
    </div>
  </div>
</div>

</body>
</html>

```

### 使用CDN
```
內容傳遞網路（英語：Content Delivery Network或Content Distribution Network，縮寫：CDN）
是指一種透過網際網路互相連接的電腦網路系統，
利用最靠近每位使用者的伺服器，更快、更可靠地將音樂、圖片、影片、
應用程式及其他檔案傳送給使用者，來提供高效能、可擴展性及低成本的網路內容傳遞給使用者。
```
```
  <script src="https://cdn.staticfile.org/jquery/3.2.1/jquery.min.js"></script>
  <script src="https://cdn.staticfile.org/popper.js/1.12.5/umd/popper.min.js"></script>
  <script src="https://cdn.staticfile.org/twitter-bootstrap/4.1.0/js/bootstrap.min.js"></script>
```
