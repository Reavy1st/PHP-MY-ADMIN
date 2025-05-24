# PHP-MY-ADMIN
Tutorial Install Php 
//database 

1, mysql -u root -p

2, Masukin password vps

3, use mysql

4, CREATE USER 'SEYZI'@'%' IDENTIFIED BY 'SEYZI';

5, GRANT ALL PRIVILEGES ON *.* TO 'SEYZI'@'%' WITH GRANT OPTION;

6, FLUSH PRIVILEGES;

7, exit

8, systemctl restart mysql

//phpyadmin 

8, export PHPMYADMIN_VERSION=$(curl --silent https://www.phpmyadmin.net/downloads/ | grep "btn btn-success download_popup" | sed -n 's/.*href="\([^"]*\).*/\1/p' | tr '/' '\n' | grep -E '^.*[0-9]+\.[0-9]+\.[0-9]+$')

9, cd /var/www/pterodactyl/public && wget https://files.phpmyadmin.net/phpMyAdmin/$PHPMYADMIN_VERSION/phpMyAdmin-$PHPMYADMIN_VERSION-all-languages.zip && unzip phpMyAdmin-$PHPMYADMIN_VERSION-all-languages.zip && rm phpMyAdmin-$PHPMYADMIN_VERSION-all-languages.zip && mv phpMyAdmin-$PHPMYADMIN_VERSION-all-languages pma

Note : Setelah itu silahkan create Di admin panel Databse username dan password sesuai Create di Atas *SEYZI* dan isi IP vps
