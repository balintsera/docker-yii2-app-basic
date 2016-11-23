# Docker Container for Yii 2.0


**Advanced App Template**

## Usage

Get it from [Docker Hub](https://registry.hub.docker.com/u/balintsera/yii2-advanced/)!

    docker pull balintsera/yii-advanced

## Development

Run the image in your application's root:

```shell
   docker run -d \
    -v `pwd`:/app \
    --name yii-adv \
    -p 8080:8080 \
    -p 8081:8081 \
    --link mariadb:mariadb \
    balintsera/yii-advanced
```

Access the application under the URLs mentioned above, you can directly edit the files of your application or run commands like

    docker exec myapp ./yii

directly off the running container.

Links
-----

- [yii2-app-basic](https://github.com/yiisoft/yii2-app-basic)
- [Phundament 4](http://phundament.com)
- [diemeisterei GmbH](http://diemeisterei.de)
