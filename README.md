# Psalm v5.1.3 Alpine Linux Issue Demo

## Setup

```shell
$ composer install
```

## Replicate Issue

```shell
$ docker run --rm -v $(pwd):/app -w /app php:8.2-alpine php vendor/bin/psalm
```

## Confirm Issue Not Present in Non-Alpine Image

```bash
$ docker run --rm -v $(pwd):/app -w /app php:8.2 php vendor/bin/psalm
```
