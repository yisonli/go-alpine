FROM golang:alpine

MAINTAINER Yison.Li <yisonli@vip.qq.com>
ENV GOPATH=/root:$GOPATH

RUN apk add bash git && \
go get github.com/astaxie/beego && \
go get github.com/beego/bee && \
cd /go/src && \
git clone https://github.com/yisonli/golang.org.git && \
go get github.com/silenceper/wechat && \
go get github.com/go-sql-driver/mysql 


