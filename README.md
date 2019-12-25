1、 生成伺服器私鑰
openssl genrsa -out server.key 2048

2、 生成伺服器證書
openssl req -new -x509 -key server.key -out server.pem -days 3650

3、 生成客戶端私鑰
openssl genrsa -out client.key 2048

4、 生成客戶端證書
openssl req -new -x509 -key client.key -out client.pem -days 3650
