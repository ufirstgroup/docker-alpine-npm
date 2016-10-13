# docker-alpine-npm

```bash
docker run -it --rm \
  -e USER_ID=`id -u` \
  -v $HOME:/homedir \
  -v `pwd -P`:/workdir  \
  ufirstgroup/alpine-npm:6.8.0_3.10.8 npm
```
