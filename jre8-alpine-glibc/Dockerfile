FROM quay.io/rubenqba/openjdk-8-jre-alpine

curl -sL https://circle-artifacts.com/gh/andyshinn/alpine-pkg-glibc/6/artifacts/0/home/ubuntu/alpine-pkg-glibc/packages/x86_64/glibc-2.21-r2.apk -o /tmp/glibc-2.21-r2.apk && \
	apk update && \
	apk add --allow-untrusted /tmp/glibc-2.21-r2.apk && 
	rm /tmp/glibc-2.21-r2.apk
