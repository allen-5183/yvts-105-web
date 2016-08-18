# 使用 CSS 控制頁面

1. 嵌入式樣式(行內樣式): 直接寫在標籤 &lt;h2&gt; 的屬性="值" 上.  
   ``` 
   <h2 style="color:red;"> Hello </h2>
   
   ```      
   <h2 style="color:red;"> Hello </h2>      
2. 內部樣式: &lt;style&gt; 標籤, 寫在網頁內容裏. 
   ```
   <style type="text/css">
      h2{                                
          color: red;                    
        }                                 
   </style>

   ```
3. 外部樣式: <link> 標籤, 將 CSS 寫在另一個檔案. 
   使用時機: 所有頁面都採用相同CSS 時.
   
   CSS: style.css
   ```
   h2{
          color:red;
   }
   ```
   HTML:
   ```
    <link rel="stylesheet" type="text/css" href="style.css" media="screen">
   ```
   
 4. 導入式: 作用相同於外部式.  
    ```
    <style type="text/css">
      <!--
        @import url(style.css)
	  -->
	</style>
    ``` 
   rel="stylesheet"   表示這是一個 CSS 檔案的參照
   href="style.css"   CSS 檔案所在位置(目錄與檔名)
   type="text/css"    指定為純文字檔
   media: 指定 CSS 是針對哪一媒體來撰寫
          screen   螢幕上的網頁
	      print    印出的結果
	      handheld 手持式週邊(行動設備)
	      default  適用各種狀況
   ```  

