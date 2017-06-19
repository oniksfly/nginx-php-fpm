## Available Configuration Parameters
The following flags are a list of all the currently supported options that can be changed by passing in the variables to docker with the -e flag.

 - **WEBROOT** : Change the default webroot directory from `/var/www/html` to your own setting
 - **ERRORS** : Set to 1 to display PHP Errors in the browser
 - **HIDE_NGINX_HEADERS** : Disable by setting to 0, default behaviour is to hide nginx + php version in headers
 - **PHP_MEM_LIMIT** : Set higher PHP memory limit, default is 128 Mb
 - **PHP_POST_MAX_SIZE** : Set a larger post_max_size, default is 100 Mb
 - **PHP_UPLOAD_MAX_FILESIZE** : Set a larger upload_max_filesize, default is 100 Mb
 - **DOMAIN** : Set domain name for Lets Encrypt scripts
 - **REAL_IP_HEADER** : set to 1 to enable real ip support in the logs
 - **REAL_IP_FROM** : set to your CIDR block for real ip in logs
 - **RUN_SCRIPTS** : Set to 1 to execute scripts
 - **PGID** : Set to GroupId you want to use for nginx (helps permissions when using local volume)
 - **PUID** : Set to UserID you want to use for nginx (helps permissions when using local volume)
 - **REMOVE_FILES** : Use REMOVE_FILES=0 to prevent the script from clearing out /var/www/html (useful for working with local files)
