# wordpress-mysql-php-ec2
 Latest version PHP,MYSQL,WORDPRESS>

    1 sudo yum update -y
    2  sudo yum install httpd -y
    3  sudo yum enable httpd
    4  sytemctl enable httpd
    5  systemctl enable httpd
    6 sudo  yum install mysql
    7  amazon-linux-extras install php7.2
    8  wget http://wordpress.org/latest.tar.gz
    9  tar -xzvf latest.tar.gz
   10  ls
   11  sudo cp -r wordpress/* /var/www/html/
   12  cd /var/www/html
   13  sudo cp wp-config-sample.php wp-config.php
   14  sudo vim wp-config.php
   15  sudo chmod -R 755 wp-content
   16  sudo chown -R apache:apache wp-content
   17  sudo systemctl enable httpd.service
   18  sudo systemctl restart httpd
   19  sudo vim wp-config.php
   20  sudo systemctl restart httpd
   22  history

define( 'FS_METHOD','direct');
