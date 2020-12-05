Install phpunit

```
docker run --rm -it --user $(id -u):$(id -g) --volume "$PWD:/app" composer:2.0.7 require "phpunit/phpunit:~9.5"
```

Enjoy

```
docker run --rm -it --user $(id -u):$(id -g) --volume "$PWD:/app" php:8.0-cli php /app/vendor/bin/phpunit /app/tests
```
