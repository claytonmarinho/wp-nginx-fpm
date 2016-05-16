
```
### Install Extra Modules
If you wish to install extras at boot time, such as extra php modules you can specify this by adding the DEBS flag, to add multiple packages you need to space separate the values:
```
sudo docker run --name nginx -e 'DEBS=php5-mongo php-json" -p 8080:80 -d richarvey/nginx-php-fpm
```

## Logging and Errors

### Logging
All logs should now print out in stdout/stderr and are available via the docker logs command:
```
docker logs <CONTAINER_NAME>
```
### Displaying Errors
If you want to display PHP errors on screen (in the browser) for debugging purposes use this feature:
```
-e ERRORS=1
```
