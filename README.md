### 使用方法：
```
cp .example.env .env

openssl dhparam -out ./www/ssl/dhparam.pem 2048

docker-composer up -d
```