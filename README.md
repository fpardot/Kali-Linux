# Kali Linux

## Descarga

Para obtener la ISO de nuestro sistema operativo Kali Linux, nos dirigimos a la página oficial de Kali, la cual encuentras en el siguiente link [Kali Linux](https://www.kali.org/get-kali/#kali-installer-images)

Bajamos hasta la sección que dice Kali Linux 2022.4 Changelog (Como se muestra en la foto)

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/2.png)

Y descargamos presionando en el icono de la flecha hacia abajo. (La ISO tiene un peso aproximado de 4 GB, el tiempo de descarga dependerá de tu conexión a internet), una vez descargada, verificamos que se encuentre el ISO.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/4.png)

## Creación de máquina virtual

Para comenzar con la instalación, es necesario que tengamos instalado un virtualizador en nuestro equipo, en este caso ocuparemos VMware 16 Player, si no saben cómo instalar VMware, puede ver mi otra publicación [Como instalar VMware](https://github.com/fpardot/VMware).

Ejecutamos WMware 16 Player

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/5.png)

Dentro de VMware, pinchamos donde dice Create a New Virtual Machine

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/6.png)

Seleccionamos donde dice **Installer disc image file (iso)** y pinchamos el botón Browse... dentro buscamos en la dirección donde descargamos la ISO de Kali Linux, en mi caso la carpeta Descargas

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/8.png)

En la siguiente pantalla seleccionamos el tipo de Sistema Operativo que queremos instalar, en nuestro caso Linux y damos a siguiente

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/9.png)

Agregamos el nombre a nuestra máquina virtual, colocamos Kali Linux (usted puede agregar el nombre que usted quiera, pero lo importante es que el nombre le sea fácil identificar la máquina que está creando) y pinchamos el botón Next >

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/10.png)

En esta sección debemos elegir la cantidad de espacio asignado al disco duro, en el cual le daremos 40 GB (No necesariamente el sistema ocupara los 40 GB, por lo cual este es un espacio reservado que podría llegar a ocupar los 40 GB, pero solo será descontado el espacio que ocupe el sistema) aproximadamente de 15 a 20 GB.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/11.png)

Damos clic en Finish y con esto tenemos creada la máquina virtual.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/13.png)

## Instalación

Una vez creada la máquina virtual, comenzaremos a instalar el sistema operativo, para esto pinchamos la máquina recién creada, y apretamos el botón Play, esto encenderá la máquina y podremos iniciar la instalación.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/14.png)

Con el teclado seleccionamos la opción **Graphical install**, el cual permitirá instalar Kali en modo gráfico.

El siguiente paso es seleccionar en que idioma queremos instalar el Sistema operativo, en mi caso seleccionare **Spanish - Español** y damos clic al botón Continue.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/15.png)

Seleccionamos el país de su residencia, para que tome de manera correcta la fecha y la hora de su zona horaria, en mi caso escogeré **Chile**

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/16.png)

El siguiente paso es muy importante, acá debemos elegir el idioma para la distribución de nuestro teclado, esto es importante para poder tener correctamente ubicado cada botón con sus respectivas letras y caracteres, en el caso de mi teclado la distribución es Latinoamericano

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/17.png)

En el nombre de máquina podemos colocar cualquier nombre, este nombre nos servirá para poder identificar la máquina en nuestra red interna.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/19.png)

En el caso de tener un nombre de Dominio, lo debes agregar en la siguiente pantalla

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/20.png)

Configuramos el nombre, el usuario y la contraseña para nuestro sistema operativo

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/23.png)

Se debe configurar la zona horaria para el reloj, en Chile nos muestras dos zonas, Santiago de Chile e Isla de pascua, en nuestro caso seleccionaremos Santiago de Chile

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/24.png)

En las siguientes pantallas seleccionaremos el particionado del disco, seleccionaremos **Guiado - utilizar todo el disco**

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/25.png)

Nos pedirá seleccionar el disco a particionar en este caso tenemos uno, pero si tuvieras más de uno deberás seleccionar cuidadosamente en cual quieres realizar la instalación, para no perder los archivos que puedas tener almacenados.

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/26.png)

En la siguiente sección nos muestra varias opciones de particionar, la primera realiza la partición automáticamente, en la segunda permite separar la partición /home, y la tercera opción es para crear una instalación más personalizada, en este caso no necesitamos realizar particiones personalizadas, como si lo haráamos en una instalación para un servidor, por lo cual elegiremos la primera opción y damos clic en Continuar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/27.png)

Seleccionamos la opción **Finalizar el particionado y escribir los cambios en el disco** y apretamos continuar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/28.png)

Nos preguntara si deseamos escribir los cambios y pinchamos en si y damos clic en continuar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/29.png)

El sistema comenzara a instalarse

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/30.png)

Nos mostrara una pantalla con los programas que queremos instalar, seleccionamos las de la foto y damos clic en continuar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/31.png)

El sistema continúa con la instalación

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/32.png)

El sistema nos preguntara si deseamos instalar el cargador de arranque GRUB, al cual debemos dar que **Si**, en el caso de colocar que **No** el sistema no iniciara

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/33.png)

Seleccionaremos donde queremos instalar el cargador de arranque

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/34.png)

Instalación completada, el Sistema operativo nos pide reiniciar el sistema y damos clic en continuar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/36.png)

Ya tenemos el sistema instalado y listo para ocupar, para esto ingresaremos el nombre de usuario y contraseña que creamos en pasos anteriores y damos clic en iniciar sesión

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/37.png)

Sistema listo para ocupar

![alt text](https://github.com/fpardot/Kali/blob/161407f4d4992be149e482badefbb8530a0b9f01/img/38.png)
