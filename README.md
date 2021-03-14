## wget
#vamos a explicar la función wget
Primero vamos a ver para que sirve la funcion wget
Wget es una herramienta informática creada por el Proyecto GNU. Puedes usarlo para recuperar contenido y archivos de varios servidores web. El nombre es una combinación de World Wide Web y la palabra get. Admite descargas a través de FTP, SFTP, HTTP y HTTPS.

Wget se crea en C portátil y se puede usar en cualquier sistema Unix. También es posible implementarlo en Mac OS X, Microsoft Windows, AmigaOS y otras plataformas populares.
Para empezar tendremos que instalar el wget con el siguiente comando:
apt-get install wget

#vamos a ver las distintas funciones del wget:
###Usar el comando Wget para guardar archivos en el directorio especificado
para eso usaremos la funcion -P:
wget -P documents/archives/ https://wordpress.org/latest.zip
###Usar el comando Wget para limitar la velocidad de descarga:
Con wget, también puedes limitar la velocidad de descarga. Esto es útil cuando recuperas archivos grandes y evitará que use todo tu ancho de banda. Este ejemplo de wget establecerá el límite a 500k:
wget --limit-rate=500k https://wordpress.org/latest.zip
###Uso del comando Wget para establecer cantidad de reintento
Los problemas de conexión a Internet pueden hacer que la descarga se interrumpa. Para abordar este problema, podemos aumentar la cantidad de reintentos usando la función -tries:
wget -tries=100 https://wordpress.org/latest.zip
###Usar el comando Wget para descargas en segundo plano:
Para archivos extremadamente grandes, puede aprovechar la función -b. Descargará su contenido en segundo plano.
wget -b http://example.com/beefy-file.tar.gz
###Usando el comando Wget para descargar a través de FTP
El comando también se puede usar con FTP. Solo necesitarás especificar el nombre de usuario y la contraseña como en este ejemplo:
wget --ftp-user=YOUR_USERNAME --ftp-password=YOUR_PASSWORD ftp://example.com/something.tar
![imagen](C:\Users\juans\OneDrive\Escritoriogracias-por-su-atencion-9.jpg)
