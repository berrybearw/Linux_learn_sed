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

<details>
<summary>取代完存取</summary>
![image](https://user-images.githubusercontent.com/96226780/201519271-a82f498b-8d0b-4738-9188-8ab994f05bd0.png)  
</details>
<details>
<summary>全部取代</summary>
![image](https://user-images.githubusercontent.com/96226780/201519295-0e14d1c5-7860-41e7-ad78-0ee871b21763.png)  
</details>
<details>
<summary>常用</summary>
![image](https://user-images.githubusercontent.com/96226780/201519314-ef497037-ad04-4513-9447-594a58738db1.png)  
</details>
<details>
<summary>sed 和 tr 取代 不同處</summary>
![image](https://user-images.githubusercontent.com/96226780/201519331-2b179b25-5b98-4845-bd3c-af7b87a4dd8a.png)
![image](https://user-images.githubusercontent.com/96226780/201519335-30dff1da-cc6e-478d-921c-b23caca921cd.png)  
</details>
<details>
<summary>逗號取代換行</summary>
![image](https://user-images.githubusercontent.com/96226780/201519314-ef497037-ad04-4513-9447-594a58738db1.png)  
</details>
<details>
<summary>逗號取代換行</summary>
![image](https://user-images.githubusercontent.com/96226780/201519358-36d8405c-6a60-4029-8c14-4300ce5370bb.png)
![image](https://user-images.githubusercontent.com/96226780/201519365-ded55033-9118-484a-9b60-5d2a20ff7bc3.png)
![image](https://user-images.githubusercontent.com/96226780/201519369-0b705b47-7155-4b37-b4b3-79b9842e8b4e.png)  
</details>
<details>
<summary>逗號取代換行</summary>
![image](https://user-images.githubusercontent.com/96226780/201519383-9b77d373-87b2-4e1b-ac5c-41bda1828bff.png)  
</details>
<details>
<summary>在檔案最後一行加上說明</summary>
參數 存檔用 -i -e 
檔案最後一行$
新增 a
換行 \
`sed -i -e '$a#2022/11/1 for 18 ora add (s)\
dbi.default.driver="dbmora_12"\
#2022/11/1 for 18 ora add (e)' fglprofile.t30std`  
![image](https://user-images.githubusercontent.com/96226780/201519415-ab6487a8-62b0-4827-94b0-50b7acd7a09e.png)
</details>
