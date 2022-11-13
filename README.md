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
