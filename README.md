# SDP IO18

## `Local` Deployment tips:

1. download and install: https://windows.php.net/download#php-8.3
    1. extract & add that folder to `C:\Program Files` `C:\Program Files\php-8.3.7` (renamed the extracted file to just php-8.3.7)
2. Install https://getcomposer.org/Composer-Setup.exe
3.

```shell
composer update --ignore-platform-reqs
```

## Production Deployment

-   https://youtu.be/kG8RP6Rk0K8?si=zrclv7haFzHnZPW4
-   https://youtu.be/kstcGqmzow8?si=eBM337XfxSwQOa6r `digital ocean`

---

## Add database

```shell
mysql -u root -p
```

password: `press enter`

```shell
show databases;
```

```shell
# adding the SQL file to the MySQL database
mysql -u root -p ecommerce < C:\Users\ASUS\Downloads\database.sql
```

> in case of probelms: [refer](https://www.youtube.com/watch?v=0Wm3KcVFMBA)

---

## Known errors:

```
Fatal error: Composer detected issues in your platform: Your Composer dependencies require a PHP version ">= 8.2.0". You are running 8.1.10. in C:\laragon\www\sdp-multivendor-ecom\vendor\composer\platform_check.php on line 24
```

### Fixes:

-   https://github.com/leokhoa/laragon/issues/600#issuecomment-1881062927
-   https://github.com/leokhoa/laragon/issues/600#issuecomment-1993504755
