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
  comando largo
  
  cd /etc/apache/services-available
  
  
4
