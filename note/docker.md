# Docker 

<br>

## ⚙️ 명령어

### Docker 파일로 이미지 빌드
```sh
# 1. 우선 Dockerfile이 있는 디렉토리 위치로 이동.
# 2. 이동 후 아래 명령어 실행
> docker build . -t '설정할 이미지 이름'
```

### 생성된 이미지 실행 (컨테이너 생성)
```sh
> docker run '옵션' '이미지 이름'
```

|옵션|설명|
|---|---|
|--name `이름`|컨테이너 이름 지정|
|-d|컨테이너를 백그라운드로 실행|
|-it|CLI 환경을 실행|
|-e `환경변수`|환경변수 지정|
|-p `외부포트`:`도커포트`|포트 바인딩|
|-v ${PWD}`로컬경로`:`컨테이너경로`|볼륨 설정/파일 마운트|

### 이미지 확인
```sh
> docker images
```

### 이미지 삭제
```sh
> docker rmi '이미지 이름'
```

### 생성된 컨테이너 조작
```sh
# 컨테이너 중지
> docker stop '컨테이너 이름'

# 컨테이너 시작
> docker start '컨테이너 이름'

# 컨테이너 재시작
> docker restart '컨테이너 이름'

# 컨테이너 로그 확인
> docker logs '컨테이너 이름'
```

### 컨테이너 확인
```sh
> docker ps     # 실행중인 컨테이너
> docker ps -a  # 모든 컨테이너
```

### 컨테이너 삭제
```sh
> docker rm '컨테이너 이름'
```

<br>

## 참고 사이트

### Docker 설치법
- https://goddaehee.tistory.com/251

### Docker Desktop 오류

- https://forums.docker.com/t/docker-failed-to-initialize/111341