FROM alpine:3.10

MAINTAINER Yison.Li <yisonli@vip.qq.com>

# 运行环境准备
RUN apk add bash ca-certificates 

# 设置时区为上海
RUN apk add tzdata && \
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone && \
    apk del tzdata
