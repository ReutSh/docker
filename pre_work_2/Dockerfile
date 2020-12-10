FROM alpine:3.9

LABEL maintainer="shwartza@gmail.com"

COPY . /src

WORKDIR /src

RUN apk update && apk upgrade && apk add python3 

RUN pip3 install -r requirements.txt

EXPOSE 5000

ENTRYPOINT [ "python3", "./app.py" ] 
