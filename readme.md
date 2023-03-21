# A PrestaShop Docker Compose Starter Project

### Follow these steps to get started:

```shell
git clone https://github.com/VidalGuilherme/docker-prestashop

cd docker-prestashop

docker-compose up -d --build
```

### Continue install:

* go to localhost (http://localhost:8585)
* follow the install steps
* use these credentials 
    * server: mysql
    * database: prestashop
    * user: prestashop
    * password: prestashoppass

### When install is finished do some clean-up:

```shell
docker exec -it prestashop-cont /bin/bash

rm -rf install
mv admin/ admin12345/

exit
```

### Now you have all access

* store: http://localhost:8585
* admin panel: http://localhost:8585/admin12345

### Restart your containers

```shell
docker-compose down --remove-orphans && docker-compose up -d
```

## What is PrestaShop

PrestaShop is a free and open-source e-commerce web application, committed to providing the best shopping cart experience for both merchants and customers. It is written in PHP, is highly customizable, supports all the major payment services, is translated in many languages and localized for many countries, has a fully responsive design (both front and back office), etc. See all the available features.

> [www.prestashop-project.org](https://www.prestashop-project.org/)