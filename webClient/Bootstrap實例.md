###
有關Bootstrap的說明ㄝ下列何者為非?
```
Bootstrap 是全球最受歡迎的前端元件庫，用於開發回應式佈局、移動設備優先的 WEB 專案。

Bootstrap4 目前是 Bootstrap 的最新版本，是一套用於 HTML、CSS 和 JS 開發的開源工具集。
利用提供的 Sass 變數和大量 mixin、回應式柵格系統、可擴展的預製元件、
基於 jQuery 的強大的外掛程式系統，
能夠快速為你的想法開發出原型或者構建整個 app 。
```


# Bootstrap 4 的網格系統
```
Bootstrap 4 的網格系統是回應式的，列會根據螢幕大小自動重新排列。

網格類
Bootstrap 4 網格系統有以下 5 個類:
.col- 針對所有設備
.col-sm- 平板 - 螢幕寬度等於或大於 576px
.col-md- 桌面顯示器 - 螢幕寬度等於或大於 768px)
.col-lg- 大桌面顯示器 - 螢幕寬度等於或大於 992px)
.col-xl- 超大桌面顯示器 - 螢幕寬度等於或大於 1200px)

Bootstrap4 網格系統規則:

網格每一行需要放在設置了 .container (固定寬度) 或 .container-fluid (全屏寬度) 類的容器中，這樣就可以自動設置一些外邊距與內邊距。
使用行來創建水準的列組。
內容需要放置在列中，並且只有列可以是行的直接子節點。
預定義的class如 .row 和 .col-sm-4 可用於快速製作網格佈局。
列通過填充創建列內容之間的間隙。 這個間隙是通過 .rows 類上的負邊距設置第一行和最後一列的偏移。
網格列是通過跨越指定的 12 個列來創建。 例如，設置三個相等的列，需要使用用三個.col-sm-4 來設置。
```
# 學習範例一:
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
//網格每一行需要放在設置了 .container (固定寬度) 或 .container-fluid (全屏寬度) 類的容器中
<div class="container">
//使用預定義的class(.row)可用於快速製作網格佈局。
  <div class="row">
//使用預定義的class(col-sm-4) 可用於快速製作網格佈局。
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
