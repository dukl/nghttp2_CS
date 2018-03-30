# nghttp2_CS
实现ubuntu系统下，基于c语言库的http2协议，简单的pc端 CS通信

运行libevent-server需要privkey.pem 和 cacert.pem 文件
运行方式：
./libevent-server 10020(port) privkey.pem cacert.pem

privkey.pem 和 cacert.pem文件生成方式：
openssl genrsa -out privkey.pem 2048
openssl req -new -x509 -key privkey.pem -out cacert.pem -days 1095
