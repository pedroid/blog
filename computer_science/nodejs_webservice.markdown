#Build your web service with node.js

##POST and GET operation

##template your html

##user ejs to render your file

###ejs 是什麼
一個將資料與網頁檔分離的platform，使用者可以專心於建構資料，而將資料嵌入網頁檔的過程叫作Render，ejs將資料作為變數。以操作流程來說明ejs：

1. 使用者發出GET要求
2. Server收到GET後，render 一個ejs檔案，同時傳入需要的資料

ejs檔案是一個有html外觀，但可以使用javascript來render變數的檔案格式

###這個平台上的blog並沒有採用ejs 架構
render適合有固定相對位置、固定風格的資料，但是因為blog的內容從markdown 轉換成html時就可以被視為一個完整的、封裝後的多媒體檔案，所以在這個平台的blog系統上並沒有使用ejs。
###那什麼時候適合用rendering ejs呢？
當多個頁面，內含有幾個影片檔、幾個圖片檔，幾段文字，這些資訊都被完整定義，而且各別儲存時，就適合用ejs的方式來render頁面。比如一般查詢資料庫的頁面

##websocket