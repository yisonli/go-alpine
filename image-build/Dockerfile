FROM golang:alpine

MAINTAINER Yison.Li <yisonli@vip.qq.com>

# 项目需要的相关go依赖包
RUN apk add bash git && \
    go get github.com/astaxie/beego && \
    go get github.com/beego/bee && \
    cd /go/src && \
    git clone https://github.com/yisonli/golang.org.git && \
    go get github.com/silenceper/wechat && \
    go get github.com/go-sql-driver/mysql 

# 设置时区为上海
RUN apk add tzdata && \
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone && \
    apk del tzdata

ENV GOPATH=/root:$GOPATH

