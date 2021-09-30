# INSTALACIÓN DE MAVEN EN UBUNTU

# 1. Introducción

En esta tarea se realizará la instalación de Apache Maven en una máquina virtual con el Sistema Operativo (SO) Ubuntu 20.

Así pues, Apache Maven es un software destinado a la compresión y gestión de proyectos creados en Java. Siendo , el objetivo principal de Maven es optimizar el trabajo del desarrollador, por medio de (Apache Maven, 2021):

- Facilitación del proceso de construcción

- Proporciona un sistema de construcción uniforme

- Proporciona información de calidad sobre el proyecto

- Fomenta las buenas prácticas de desarrollo

Una vez dicho esto a continuación se desarrollará la instalación de Apache Maven dentro de una máquina virtual con el SO Ubuntu 20.

 # 2.  Instalación de Apache Maven
 
 Para realizar la instalación del software se utilizará el terminal (no se descargará nada de la página de Apache Maven). Dentro del terminal se utilizará en primer lugar el comando que se muestra a continuación para actualizar el índice del paquete, necesario para la instalación del programa (Fig.1.):
 
 **<p align="center"> sudo apt update </p>**
 
 ![Figura.1. Ventana del terminal donde se ve reflejado el comando necesario para la actualización del paquete. [Elaboración propia]](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/1M.png "Figura.1. Ventana del terminal donde se ve reflejado el comando necesario para la actualización del paquete. [Elaboración propia]")

Una vez actualizado el paquete se procederá a la instalación de Maven. Para ello se utilizará el comando:

**<p align="center"> sudo apt install maven </p>**

Una vez introducido el comando dará inicio la instalación como bien se puede observar en la figura 2 y 3.

 ![Figura.2.Ventana del terminal donde se muestra la instalación completa de Apache Maven. [Elaboración propia]](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/2M.png "Figura.2.Ventana del terminal donde se muestra la instalación completa de Apache Maven. [Elaboración propia]")
 
  ![Figura.3. Finalización de la instalación de Apache Maven. [Elaboración propia]](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/4M.png "Figura.3. Finalización de la instalación de Apache Maven. [Elaboración propia]")

Una vez hecho esto verificaremos la versión de Maven que se ha instalado por medio del comando:

**<p align="center"> mvn -version </p>**

Así pues, y como bien se muestra en la figura 4, en este caso la versión de Maven será la 3.6.3, no siendo esta la más reciente.

  ![Figura.4.  Comprobación de la versión de Maven. [Elaboración propia]](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/6M.png "Figura.4.  Comprobación de la versión de Maven. [Elaboración propia]")
  
  ## 2.1 Instalación de una versión concreta de Maven
  
Para llevar a cabo una instalación de una versión concreta de Maven será necesario descargar la versión deseada de Apache Maven en la carpeta temporal (/tmp) a través del comando:

**<p align="center"> wget https://www.apache.org/dist/maven/maven-3/3.8.2/binaries/apache-maven-3.8.2-bin.tar.gz -P /tmp </p>**

Este comando estaría destinado a la descarga del Apache Maven 3.8.2, por lo que si se quisiera utilizar otra versión sería necesario cambiar parte del comando.

  ![Figura.5. Ventana del terminal con el comando necesario para descargar la versión 3.8.2 de Maven. [Elaboración propia]
](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/7M.png "Figura.5. Ventana del terminal con el comando necesario para descargar la versión 3.8.2 de Maven. [Elaboración propia]")

 ![Figura.6. Ventana del terminal donde se muestra la finalización de la descarga de Maven 3.8.2.[Elaboración propia]
](https://raw.githubusercontent.com/jdabrante/INFORME-N-2/DAW/8M.png "Figura.6. Ventana del terminal donde se muestra la finalización de la descarga de Maven 3.8.2.[Elaboración propia]")

Una vez finalizada la descarga (figura 5 y 6) se podrá proceder a la extracción del archivo en el directorio /opt a través del comando:

**<p align="center"> sudo tar xf /tmp/apache-maven-*.tar.gz -C /opt </p>**

Hay que tener en cuenta que con este comando no se ve reflejada ninguna acción dentro del terminal, por lo que tendremos que comprobar que efectivamente se ha realizado la descompresión del archivo en el directorio /opt

Además es importante tener en cuenta que en el comando anteriormente citado el * corresponde a la versión de Maven.










