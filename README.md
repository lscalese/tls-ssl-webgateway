# tls-ssl-webgateway

This is a simple script to build a docker image in order to use Intersystems Webgateway with HTTPS and SSL\TLS support with IRIS instance.  

This small project is a dependence for : 

 * [iris-mirroring-with-webgateway](https://github.com/lscalese/iris-mirroring-with-webgateway)


# Build tls-ssl-webgateway

```bash
git clone https://github.com/lscalese/tls-ssl-webgateway
cd tls-ssl-webgateway
docker login -u="YourWRCLogin" -p="YourPassWord" containers.intersystems.com
docker pull containers.intersystems.com/intersystems/webgateway:2021.1.0.215.0
docker build --no-cache -t tls-ssl-webgateway .
```
# Links

A sample is available on [docker-webgateway-sample](https://github.com/lscalese/docker-webgateway-sample) repository.  