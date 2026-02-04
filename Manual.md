# Manual Técnico
### Luis Emilio Rivera Yurrita - 202004712
### Practica 1
### Laboratorio de Sistemas Operativos 2

## Configuración de VMWare

Lo primero que se debe hacer es instalar VMWare, ya que este nos servirá para crear la máquina virtual, a su vez, debemos descargar la ISO de Linux Mint deseada.

Una vez se tenga instalado el VMWare y descargada la ISO, se debe proceder a configurar la máquina virtual.

![Imagen1](imgs/1.png)

Para crear la VM vamos a dar clic en la opción de "Custom(advanced)", para poder crear la máquina virtual con libertad para asignar los recursos requeridos.

![Imagen2](imgs/2.png)

![Imagen3](imgs/3.png)

Se decide la ruta donde estará almacenada la máquina virtual

![Imagen4](imgs/4.png)

Se selecciona la versión de Linux que vamos a instalar, en este caso, al no aparecer la versión de Linux Mint, se usa Ubuntu 64-bit ya que este esta basado en Ubuntu.

![Imagen5](imgs/5.png)

Se le da un nombre a la máquina virtual y se confirma la localización donde estará la misma.

![Imagen6](imgs/6.png)

Ahora se elige la cantidad de procesadores y nucleos que tendrá, en este caso se eligieron 2 procesadores de 1 núcleo cada uno.

![Imagen7](imgs/7.png)

Se debe elegir la cantidad de memoria RAM que tendrá, en este caso, se eligieron 4 GB (4096 MB).

![Imagen8](imgs/8.png)

Para el tipo de conexión, se selecciona la por defecto, que en este caso es la NAT.

![Imagen9](imgs/9.png)

Para el tipo de controladores dejaremos el por defecto, que sería el LSI logic.

![Imagen10](imgs/10.png)

Para el tipo de disco dejamos el recomendado que es el SCSI.

![Imagen11](imgs/11.png)

Se elige la opción de crar un nuevo disco virtual.

![Imagen12](imgs/12.png)

Se especifica el espacio que tendrá el disco virtual, que en este caso con 20 GB será mas que suficiente.

![Imagen13](imgs/13.png)

Se confirma el nombre que tendrá el disco virtual.

![Imagen14](imgs/14.png)

Se confirma toda la información de la máquina virtual con el resumen, y si todo es correcto, se confirma.

## Instalación del sistema operativo

![Imagen15](imgs/15.png)

Una vez confirmamos, nos mostrará la pantalla de arranque del sistema operativo, y elegiremos la opción de iniciar Linux Mint.

![Imagen16](imgs/16.png)

Se selecciona el idioma.

![Imagen17](imgs/17.png)

Marcamos la opción para instalar "Multimedia Codecs".

![Imagen18](imgs/18.png)

Se elige el tipo de instalación, en este caso elegiremos la de borrar el disco e instalar Linux Mint, esto no dará problema ya que al estar en la máquina virtual, esta usa el disco virtual que fue creado para ella.

![Imagen19](imgs/19.png)

Se selecciona la ubicación

![Imagen20](imgs/20.png)

Elegimos nombre de usuario y contraseña.

![Imagen21](imgs/21.png)

Procedemos a reiniciar la máquina virtual una vez se completa la instalación del sistema operativo.

![Imagen22](imgs/22.png)

Al reiniciar, tendremos el escritorio de Linux Mint, donde ya no veremos ningún mensaje, esto indica que la instalación se dio sin problemas.

## Configuración del sistema operativo

![Imagen23](imgs/23.png)

Comando que comprueba que el kernel funciona correctamente.

![Imagen24](imgs/24.png)

![Imagen25](imgs/25.png)

![Imagen26](imgs/26.png)


![Imagen27](imgs/27.png)

Comandos para confirmar que los recursos que se asignarión a la máquina virtual son correctos.

![Imagen28](imgs/28.png)

Comando para confirmar que la conexión a la red es correcta.

![Imagen29](imgs/29.png)

Comando para agregar un nuevo usuario y ver el grupo al que pertenece, en este caso, se creo un usuario no administrador.

![Imagen30](imgs/30.png)

Para corroborar que el usuario no puede ejecutar comandos de administrador, se hace el cambio al mismo, y se ejecuta un comando, y al dar error, sabremos que es porque el usuario no tiene permisos, lo cual esta bien.

## Configuraciones extras

![Imagen31](imgs/31.png)

Se instala y se corrobora que las herramientas de gcc y git hayan sido instalados correctamente.

![Imagen32](imgs/32.png)

Se instalan las herramientas de vmware para poder habilitar el compartir archivos entre el host y la máquina virtual.

![Imagen33](imgs/33.png)

Se configura el vmware para permitir que la máquina virtual tenga permitido el compartir archivos.

![Imagen34](imgs/34.png)

Indicamos la ruta donde estará los archivos compartidos y le damos un nombre a la carpeta.

![Imagen35](imgs/35.png)

Mediante comandos, verificamos la existencia de la ruta donde estará los archivos compartidos, de no existir, la creamos, y si al volver a corroborar la ruta, obtenemos el nombre de la carpeta compartida, sabremos que fue exitoso.

![Imagen36](imgs/36.png)

Se crea un archivo de prueba en el host y se comprueba que tambien exista en la máquina virtual, de ser así, el compartir archivos funciona correcamente.