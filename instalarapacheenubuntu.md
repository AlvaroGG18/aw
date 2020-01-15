## INSTALAR EN UBUNTU 18.04 UN APACHE

### introducción Servidor Apache


$ sudo apt-get install apache2

sudo fuser -vki /var/lib/dpkg/lock

subrayado
---

*cursiva*

**negrita**

### Firewall Linux
$ sudo ufw app list

Estamos en la empresa guru.com. Allí nos han pedido que creemos una pequña página web para probar el servidor Apache que ha instalado Accenture. Pero no tenemos interfaz gráfica.

Como reiniciar el servidor Apache
  $ sudo systemctl stop apache2
  $ sudo systemctl start apache2
  
  cd /var/www
  mkdir example.com test.com
  mkdir public_html (En cada arpeta)
  index.html (Dentro de public_html)
  cp /etc/apache2/sites-available/000-default.conf /etc/apahce2/sites-available/example.com.conf
  cp /etc/apache2/sites-available/000-default.conf /etc/apahce2/sites-available/test.com.conf
  
  cd /etc/apache/services-available
  a2ensite example.com.conf
  a2ensite test.com.conf
  a2ensite 000-default.conf
  systemctl reload apache2
  service apache2 restart
  
  /etc
  nano hosts -->  10.0.2.15 example.com
                  10.0.2.15 test.com
  a2ensite example.com.conf
  a2ensite test.com.conf
  service apache2 stop
  service apache2 start
  
  
  
