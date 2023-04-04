# base image
FROM node:12.18.1-alpine

WORKDIR /usr/src/app

# 필요한 파일 복사
COPY package*.json ./

# 필요한거 설치
RUN npm install --only=production

# 소스코드 복사
COPY ./src ./src

# 파일 복사
COPY ./videos ./videos

# 애플리케이션 실행
CMD npm start