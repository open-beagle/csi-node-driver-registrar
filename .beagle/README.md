# 说明

```bash
git remote add upstream git@github.com:kubernetes-csi/node-driver-registrar.git
git fetch upstream
git merge v2.0.1
```

## BASEIMAGE

https://github.com/GoogleContainerTools/distroless/blob/master/base/README.md

```bash
# x86_64
docker pull gcr.io/distroless/base:latest && \
docker tag gcr.io/distroless/base:latest registry.cn-qingdao.aliyuncs.com/wod/distroless-base:latest && \
docker push registry.cn-qingdao.aliyuncs.com/wod/distroless-base:latest

# arm64
docker pull gcr.io/distroless/base:latest-arm64 && \
docker tag gcr.io/distroless/base:latest-arm64 registry.cn-qingdao.aliyuncs.com/wod/distroless-base-arm64:latest && \
docker push registry.cn-qingdao.aliyuncs.com/wod/distroless-base-arm64:latest
```
