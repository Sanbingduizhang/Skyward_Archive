- 使用docker build创建镜像
	- `docker build`

### docker 发布镜像
- `docker compose -f docker-compose-build-srs.yaml build`

### 对已有镜像打包发布
- `docker tag ubuntu-ffmpeg:latest 10.10.10.29:5000/ubuntu-ffmpeg:latest`
- `docker push 10.10.10.29:5000/ubuntu-srs:latest`

### docker运行
- `docker compose -p rtmp2 -f docker-compose2.yaml up -d`