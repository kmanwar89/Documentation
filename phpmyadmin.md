Using ubuntu server 16.04 LTS, I installed phpmyadmin.
Navigating to <ipaddress>/phpmyadmin yielded a 500 server error
Fixed by following advice here: http://stackoverflow.com/questions/21699774/internal-server-error-http-error-500-after-installing-phpmyadmin-on-a-certain
sudo apt-get install php-mbstring php7.0-mbstring php-gettext
Sudo service apache2 restart

