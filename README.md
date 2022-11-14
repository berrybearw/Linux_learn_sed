# Linux_learn_sed
sed 指令 ( 取代 , 截取行 )
===
删除文件第一行：

sed -i '1d' filename

删除文件最后一行：

sed -i '$d' fileName

刪除首行空白

sed 's/^[ \t]*//g'

參考 : [https://codertw.com/前端開發/393321/](https://codertw.com/%E5%89%8D%E7%AB%AF%E9%96%8B%E7%99%BC/393321/)

在檔案最後一行加上說明
---
    參數 存檔用 -i -e 
    檔案最後一行$
    新增 a
    換行 \
```Bash
sed -i -e '$a#2022/11/1 for 18 ora add (s)\
dbi.default.driver="dbmora_12"\
#2022/11/1 for 18 ora add (e)' fglprofile.t30std
```  
![image](https://user-images.githubusercontent.com/96226780/201519415-ab6487a8-62b0-4827-94b0-50b7acd7a09e.png)

取代完存取
---
![image](https://user-images.githubusercontent.com/96226780/201519271-a82f498b-8d0b-4738-9188-8ab994f05bd0.png)  

全部取代
---
![image](https://user-images.githubusercontent.com/96226780/201519295-0e14d1c5-7860-41e7-ad78-0ee871b21763.png)  

常用
---
![image](https://user-images.githubusercontent.com/96226780/201519314-ef497037-ad04-4513-9447-594a58738db1.png)  

sed 和 tr 取代 不同處
---
![image](https://user-images.githubusercontent.com/96226780/201519331-2b179b25-5b98-4845-bd3c-af7b87a4dd8a.png)
![image](https://user-images.githubusercontent.com/96226780/201519335-30dff1da-cc6e-478d-921c-b23caca921cd.png)  

逗號取代換行
---
![image](https://user-images.githubusercontent.com/96226780/201519314-ef497037-ad04-4513-9447-594a58738db1.png)  

排序後存取
---
![image](https://user-images.githubusercontent.com/96226780/201591075-70525f1b-ef12-4d8b-a2db-39496da44585.png)

處理最後一個特殊字詞
---
![image](https://user-images.githubusercontent.com/96226780/201591145-0c2f1e1f-99a5-4ee5-a2d3-5a2ed915462a.png)

假設最後一個 }, 要改成 }

![image](https://user-images.githubusercontent.com/96226780/201591171-536322ac-e286-41cc-8072-6281a629f33d.png)

先用 grep 找出第幾行

![image](https://user-images.githubusercontent.com/96226780/201591253-39764c7c-0059-4834-8940-cde33a171b37.png)

截取出 行號

![image](https://user-images.githubusercontent.com/96226780/201591365-64b4e982-5f0b-42e2-b9e3-f66b18381da3.png)

