# Для доступа из под Alpine Linux

https://gitlab.alpinelinux.org/alpine/aports/-/issues/15199

```
[ -e /dev/net ] || mkdir /dev/net
[ -e /dev/net/tun ] || (mknod /dev/net/tun c 10 200 && chmod 600 /dev/net/tun)
```
