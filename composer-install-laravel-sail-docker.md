##  Composer install usando docker

    docker run --rm \
        -u "$(id -u):$(id -g)" \
        -v $(pwd):/opt \
        -w /opt \
        laravelsail/php80-composer:latest \
        composer install --ignore-platform-reqs

 Es simplemente la mejor opción a la hora de  bajarte un repositorio de
 laravel y usar sail para montar tu aplicación

> Debes tener  en tu maquina docker y docker-compose ya configurados.
