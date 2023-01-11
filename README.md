# Docker Learning Lessons

This project is meant to be used for testing purpose to ease understand some advance Docker concepts.

## Tooling

### Dive

https://github.com/wagoodman/dive
![Image](docs/demo.gif)

### Docker history

```
┌─[jaime@jaime-mac-pro]─[/var/jaime]─[k8s|minikube]─[aws|default]
└─╾ docker history edge-gateway-gateway --no-trunc

IMAGE                                                                     CREATED        CREATED BY                                                                                                                                                                   SIZE      COMMENT
sha256:98a4ba11cf6a063f6b5e1509374b963d4b9a5682e6226e8f5e293f4e26082be5   22 hours ago   COPY pub_jwks.json /etc/krakend/jwks.json # buildkit                                                                                                                         2B        buildkit.dockerfile.v0
<missing>                                                                 22 hours ago   COPY /tmp/krakend.json . # buildkit                                                                                                                                          3.67kB    buildkit.dockerfile.v0
<missing>                                                                 7 months ago   /bin/sh -c #(nop)  EXPOSE 8000 8090                                                                                                                                          0B
<missing>                                                                 7 months ago   /bin/sh -c #(nop)  CMD ["run" "-c" "/etc/krakend/krakend.json"]                                                                                                              0B
<missing>                                                                 7 months ago   /bin/sh -c #(nop)  ENTRYPOINT ["/usr/bin/krakend"]                                                                                                                           0B
<missing>                                                                 7 months ago   /bin/sh -c #(nop) WORKDIR /etc/krakend                                                                                                                                       0B
<missing>                                                                 7 months ago   /bin/sh -c #(nop)  USER 1000                                                                                                                                                 0B
<missing>                                                                 7 months ago   /bin/sh -c #(nop) COPY file:1753d9e6e432e8d92c2cf6040943239c52da818ef9fce4b544de61f7c75c8745 in /usr/bin/krakend                                                             93.7MB
<missing>                                                                 7 months ago   /bin/sh -c apk add --no-cache ca-certificates &&     adduser -u 1000 -S -D -H krakend &&     mkdir /etc/krakend &&     echo '{ "version": 3 }' > /etc/krakend/krakend.json   500kB
<missing>                                                                 7 months ago   /bin/sh -c #(nop)  LABEL maintainer=community@krakend.io                                                                                                                     0B
<missing>                                                                 9 months ago   /bin/sh -c #(nop)  CMD ["/bin/sh"]                                                                                                                                           0B
<missing>                                                                 9 months ago   /bin/sh -c #(nop) ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in /                                                                             5.57MB
```



## General Concepts
* https://vsupalov.com/docker/


### Docker Layers
* https://vsupalov.com/docker-image-layers/
* [folder/layers/README.md](layers/README.md)

