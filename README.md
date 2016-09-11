# docker-phpcs-drupal

[![](https://images.microbadger.com/badges/version/skilldlabs/docker-phpcs-drupal.svg)](http://microbadger.com/images/skilldlabs/docker-phpcs-drupal "Get your own version badge on microbadger.com")

## How to use
Go to needed directory with code
```
cd /path/to/check
```
By default we call phpcs from container
```
docker run --rm -v $(pwd):/work skilldlabs/docker-phpcs-drupal
```

To call phpcbf you need to override default command
```
docker run --rm -v $(pwd):/work skilldlabs/docker-phpcs-drupal phpcbf --standard=Drupal .
```

## Shortening of container name

```
docker tag skilldlabs/docker-phpcs-drupal phpcs
```

then you can use `docker run --rm -v $(pwd):/work phpcs`
