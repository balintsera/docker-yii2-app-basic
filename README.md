# Docker Container for Yii 2.0


**Advanced App Template**

## Usage

Get it from [Docker Hub](https://registry.hub.docker.com/u/schmunk42/yii2-app-basic/)!

    docker pull schmunk42/yii2-app-basic

Run the container

    docker run -p 8888:80 schmunk42/yii2-app-basic

Open [http://127.0.0.1:8888](http://127.0.0.1:8888) (Linnx) or [http://192.168.59.103:8888](http://192.168.59.103:8888) (OS X, Windows) in your browser.

Use `Ctrl+c` to stop the process, you can also start the docker process in the background, by adding the `-d` or `--detach` option.

## Development

Copy the applictaion template from the image to your host, the following command will create a `myapp` app folder in your working directory.

   docker run \
    -v `pwd`:/app \
    --name yii-adv \
    -p 8080:8080 \
    -p 8081:8081 \
    --link mariadb:mariadb \
    serabalint/yii-advanced

Access the application under the URLs mentioned above, you can directly edit the files of your application or run commands like

    docker exec myapp ./yii

directly off the running container.

Links
-----

- [yii2-app-basic](https://github.com/yiisoft/yii2-app-basic)
- [Phundament 4](http://phundament.com)
- [diemeisterei GmbH](http://diemeisterei.de)
