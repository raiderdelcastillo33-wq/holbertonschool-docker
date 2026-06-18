FROM alpine
COPY message.txt /message.txt
RUN apk add --no-cache curl
CMD ["cat", "/message.txt"]
