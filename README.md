# learning-aqua-renovate-docker

docker を用いて、 local で renovate を実行する。

## 実行方法
```shell
export RENOVATE_TOKEN=${github_classic_personal_token}

# 実行 (相対パスは使えないらしいので、 `pwd`)
docker run --rm -v "`pwd`/config.js:/usr/src/app/config.js" --env RENOVATE_TOKEN renovate/renovate
```
