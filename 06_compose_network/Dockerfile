# 생성할 이미지의 base 이미지
FROM nginx:1.28-alpine

# 현재 폴더의 index.html을
# 실행되는 컨테이너에 존재하는 
# /usr/share/nginx/html/index.html 복사하기(덮어쓰기)
COPY index.html /usr/share/nginx/html/index.html

# 컨테이너 연결 내부포트를 80번으로 지정
EXPOSE 80

# 컨테이너 내부에 명렁어 입력: nginx -g daemon off;
# - nginx 전역 설정 중 daemon(백그라운드 서비스) off
CMD ["nginx", "-g", "daemon off;"]