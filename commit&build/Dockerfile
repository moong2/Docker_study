FROM ubuntu:20.04
# 빌드가 되는 시점에 진행되는 명령어 (이미지에 반영)
RUN apt update && apt install -y python3
WORKDIR /var/www/html
# RUN echo "Hello, <strong>Docker</strong>" > index.html
COPY ["index.html", "."]
# 컨테이너가 실행될 때 실행되는 명령어 (컨테이너에 반영)
CMD ["python3", "-u", "-m", "http.server"]