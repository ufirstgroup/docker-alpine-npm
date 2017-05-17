[![](https://images.microbadger.com/badges/image/ufirstgroup/alpine-npm.svg)](https://microbadger.com/images/ufirstgroup/alpine-npm "Get your own image badge on microbadger.com")

# docker-alpine-npm

```bash
docker run -it --rm \
  -e USER_ID=`id -u` \
  -e GROUP_ID=`id -g` \
  -v $HOME:/homedir \
  -v `pwd -P`:/workdir  \
  ufirstgroup/alpine-npm:7.10.0_4.5.0 npm
```
