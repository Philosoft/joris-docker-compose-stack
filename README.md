Install dependencies

```
docker run --rm -it --user $(id -u):$(id -g) --volume "$PWD:/app" composer:2.0.7 install
```

Enjoy

```
docker run --rm -it --user $(id -u):$(id -g) --volume "$PWD:/app" php:8.0-cli php /app/vendor/bin/phpunit /app/tests
```
