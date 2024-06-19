# HTML

[TOC]

---
## 創建第一個網頁
<iframe width="560" height="315" src="https://www.youtube.com/embed/4b9g8j6yL8Y?si=HjlYKeT5-uIPaXnw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


```html=
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8"></meta>
        <title>李倢的網頁</title>
    </head>
    <body>
        hello 我是李倢
    </body>
    
</html>
```
![image](https://hackmd.io/_uploads/SyQA0F0H0.png)

## 註解、基本標籤
<iframe width="560" height="315" src="https://www.youtube.com/embed/LD1PhxcYKRI?si=55K3nE7RlKly1Boq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

```html=
<!DOCTYPE html>
<html>
    <head>
        <!-- 下面那行表達的是網頁的編碼-->
        <meta charset="UTF-8"></meta>
        <title>李倢的網頁</title>
    </head>
    <body>
        <!-- 這是一個註解 -->
        hello 我是李倢
        <!-- h1-h6 都是標題 由大到小 -->
        <h3>我是一個標題</h3>
        <!-- p是段落 -->
        <p>我是一個段落</p>

        <br> <!-- br是換行 -->
        <hr> <!-- hr是水平線 -->
        
        <h3> 第二個標題 </h3>
        <!-- b是粗體 i是斜體 -->
        <p><i>斜體i</i><b>粗體b</b></p>
    </body>
    
</html>
```
![image](https://hackmd.io/_uploads/B1ZyI5CrA.png)

## 連結、圖片
<iframe width="560" height="315" src="https://www.youtube.com/embed/14Zc6hA5OP8?si=27gLKUekBTpaeBci" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

縮牌和換行都只是讓人類更容易去閱讀
其實有無縮排的執行結果都一樣
``` html=
<!DOCTYPE html>
<html>
    <head>
        <!-- 下面那行表達的是網頁的編碼 charset也是屬性 代表編碼-->
        <meta charset="UTF-8"></meta>
        <title>李倢的網頁</title>
    </head>
    <body>
       
        <!--a標籤需要屬性 => href 代表網址的屬性 -->
        <a href="https://www.google.com">google</a>
    
        <!-- 連結到自己的另外一個網頁-->
        <a href ="page2.html">第二頁</a>
        <!-- 連結到自己的不在同一個資料夾下的網頁-->
        <a href ="dir/page3.html">第三頁</a>
        <!--要注意page3連結回來的方式-->
        
        <!--連結到圖片or pdf檔是一樣的方式-->
        <a href = "me.jpg">我</a>
        <a href="第十五週作業_資管一 b12705041 李倢安.pdf">pdf</a>
        

        <!--在網頁中插入圖片-->
        <!-- src 表示屬性-->
        <!--從外部網址-->
        <img src = "https://tw.portal-pokemon.com/play/resources/pokedex/img/pm/5f27124544444c7565d9dc54c3227f3970aa7454.png" height = "300" >
        <!--從自己的資料夾 順便調整這張圖要呈現的大小-->
        <img src = "me.jpg" width="400" height="400" > <!-- width height 是屬性 圖片被壓縮了-->
        <img src = "me.jpg" width = "300"> <!--根據width 去等比例縮小-->
    </body>
    
</html>
```
![image](https://hackmd.io/_uploads/H1Hhj0CHC.png)

![螢幕擷取畫面 2024-06-18 150720](https://hackmd.io/_uploads/rkC8iARr0.png)

---

## 在網頁中插入影片 or youtube 影片
```html=
<!DOCTYPE html>
<html>
    <head>
        <!-- 下面那行表達的是網頁的編碼 charset也是屬性 代表編碼-->
        <meta charset="UTF-8"></meta>
        <title>李倢的網頁</title>
    </head>
    <body>
       
        <!--在網頁中插入影片 or youtube 影片-->
        <!-- controls 顯示出可控制影片播放的按鈕-->
        <video src = "草東大港.mp4" controls height="600">當影片載入失敗會出現的東西</video>
        <!--yt影片: 分享=>嵌入=>複製貼上 -->
        <iframe width="560" height="315" src="https://www.youtube.com/embed/HQaDd_nEb0I?si=_w1cWClQqLopa7_I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
        
    </body>
    
</html>
```
![螢幕擷取畫面 2024-06-19 183247](https://hackmd.io/_uploads/HJElK4lUC.png)
 ## 列表、表格
 ```html=
     <!--列表-->
        <!--ul是無序列表 ol是有序列表-->
        <ul>
            <li>第一個項目</li>
            <li>第二個項目</li>
            <li>第三個項目</li>
        </ul>
        <ol><!-- ol是有序列表 預設用數字排列 -->
            <li>第一個項目</li>
            <li>第二個項目</li>
            <li>第三個項目</li>
        </ol>
        <ol type="I"> <!-- type是屬性 可以改成大寫羅馬數字 -->
            <li>第一個項目</li>
            <li>第二個項目</li>
            <li>第三個項目</li>
        </ol>

        <!--表格-->
        <table width = "400"><!-- table 創立-->
            <tr><!-- tr是table row 表示一行-->
            <td>國</td> <!-- td是table data 表示一格-->
            <td>數</td>
            <td>英</td>
            </tr>
            <tr>
                <td>60</td>
                <td>60</td>
                <td>60</td>
            </tr>
            <tr>
                <td>70</td>
                <td>70</td>
                <td>70</td>
            </tr>
        </table>

```
![螢幕擷取畫面 2024-06-19 183409](https://hackmd.io/_uploads/HJ_fFNlIA.png)



## 容器 div、span
```html=
 <!--html的容器 div、span-->
        <!--div是容器 可以放很多東西 但是不會有特別的效果 但用了在之後CSS美化和排版時會好用很多-->
        <div style = "color:red;"> <!-- style是屬性 可以改變字的顏色 css語法-->
            <!--列表-->
            <!--ul是無序列表 ol是有序列表-->
            <ul>
                <li>第一個項目</li>
                <li>第二個項目</li>
                <li>第三個項目</li>
            </ul>
            <ol><!-- ol是有序列表 預設用數字排列 -->
                <li>第一個項目</li>
                <li>第二個項目</li>
                <li>第三個項目</li>
            </ol>
            <ol type="I"> <!-- type是屬性 可以改成大寫羅馬數字 -->
                <li>第一個項目</li>
                <li>第二個項目</li>
                <li>第三個項目</li>
            </ol>

            <!--表格-->
            <table width = "400"><!-- table 創立-->
                <tr><!-- tr是table row 表示一行-->
                <td>國</td> <!-- td是table data 表示一格-->
                <td>數</td>
                <td>英</td>
                </tr>
                <tr>
                    <td>60</td>
                    <td>60</td>
                    <td>60</td>
                </tr>
                <tr>
                    <td>70</td>
                    <td>70</td>
                    <td>70</td>
                </tr>
            </table>
        </div>
        <hr>

        <a href="#">link1</a> <!--只佔 本身所需的空間-->
        <a href="#">link2</a>
        <p>你好 </p> <!--佔一整行-->
        <p>哈哈</p>
        <!--span 和 div的差別-->
        <span>span1</span> <!--span 只佔 本身所需的空間-->
        <span>span2</span>
        <div>div1</div> <!--div 佔一整行-->
        <div>div2</div>
```
![image](https://hackmd.io/_uploads/Bk_TYEgUA.png =50%x)
