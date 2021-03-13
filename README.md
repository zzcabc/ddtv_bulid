# DDTV_Docker_Image_Build

[源项目地址](https://github.com/CHKZL/DDTV2)

本项目利用GitHub Action编译源码，打包成Docker镜像，自动上传至[DockerHub](https://registry.hub.docker.com/r/zzcabc/ddtv)

手动点击Star获取最新的源码，编译并上传，目前仅支持AMD64位CPU架构


使用方法
```dockerfile
docker run -d \
zzcabc/ddtv:amd64 \
-- restart always \
-p 11419:11419 \
-v {config-path}BiliUser.ini:/DDTVLiveRec/BiliUser.ini \
-v {config-path}RoomListConfig.json:/DDTVLiveRec/RoomListConfig.json \
-v {config-path}tmp:/DDTVLiveRec/tmp \
--name ddtv 
```