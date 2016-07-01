FROM centos
MAINTAINER deadwood <deadwood@example.com>

# RUN: build するときに実行される
RUN yum install -y httpd

# ADD: カレントディレクトリのファイルをコピーする
# 除外するものは .dockerignore を利用する
# ADD . /var/www/html/

# EXPOSE: Port 80 を開ける
EXPOSE 80

# CMD: RUN するときに実行される
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
