# aBive
nginx 자동 실행을 위한 추가 입력 코드
1. /etc/init.d/nginx
-> CR 제거 필요,
-> >sed -i -e 's/\r//g' /etc/init.d/nginx

2. /lib/systemd/system/nginx.service
-> CR 제거 필요,

3. chkconfig --add nginx
4. chkconfig --level 3 nginx on
5. service nginx start
