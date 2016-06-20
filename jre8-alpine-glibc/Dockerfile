FROM quay.io/rubenqba/openjdk-8-jre-alpine

RUN apk --no-cache add wget ca-certificates && \
	wget -q -O /etc/apk/keys/sgerrand.rsa.pub https://raw.githubusercontent.com/sgerrand/alpine-pkg-glibc/master/sgerrand.rsa.pub && \
	wget https://github.com/sgerrand/alpine-pkg-glibc/releases/download/2.23-r3/glibc-2.23-r3.apk && \
	apk add glibc-2.23-r3.apk
#RUN apk add --update curl ca-certificates && \
#	curl -L "https://circle-artifacts.com/gh/andyshinn/alpine-pkg-glibc/6/artifacts/0/home/ubuntu/alpine-pkg-glibc/packages/x86_64/glibc-2.21-r2.apk" -o /tmp/glibc-2.21-r2.apk && \
#    apk add --allow-untrusted /tmp/glibc-2.21-r2.apk && \
#    curl -L "https://circle-artifacts.com/gh/andyshinn/alpine-pkg-glibc/6/artifacts/0/home/ubuntu/alpine-pkg-glibc/packages/x86_64/glibc-bin-2.21-r2.apk" -o /tmp/glibc-bin-2.21-r2.apk && \
#    apk add --allow-untrusted /tmp/glibc-bin-2.21-r2.apk && \
#    /usr/glibc/usr/bin/ldconfig /lib /usr/glibc/usr/lib && \
#    rm /tmp/*.apk

# RUN apk add --update curl ca-certificates glibc 
#     /usr/glibc/usr/bin/ldconfig /lib /usr/glibc/usr/lib
