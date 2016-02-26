# Data Mining
Curso de Data Mining con Oracle 12c

##Entregable No.1
Instalación de Oracle 12c y de SQL Developer 4.1.x. Para ello sólo deberás de proporcionar las impresiones de pantalla de cada uno de los pasos de la instalación en un documento  de texto.
![Primer entregable](http://shotcretemexico.com/cursos/base-datos/entregable1.png)
##Entregable No. 2

###Introducción
El objetivo de la minería de datos es analizar los datos acumulados a lo largo de varios añosde operación de las empresas. Esto es, hacer análisis de los datos a un nivel **estratégico** y a un nivel **operativo**.
Para ello es necesario primeramente preparar los datos para ese análisis (Datawarehousing), ya que las bases de datos normalizadas son bastante difíciles de manejar, sobre todo cuando se trata de hacer análisis estádisticos tanto inferenciales, como de tipo pronóstico (tendencias a futuro de la información de los datos).

Recuerda que la normalización es un proceso que debe de llevarse a cabo en la creacion de una base  de datos a un nivel **operativo** para garantizar la **integridad de datos**. Sin embargo al tratar de  analizar grandes cantidades de datos resulta muy ineficiente tener los datos en este tipo de formato, ya que el uso de **joins** para manejar multiples campos de distintas tablas se hace casi imposible o muy difícil de llevar a cabo.
Para resolver ese conflicto y poder hacer un análisis de datos (minería de datos) con las técnicas que veremos en este curso,  es necesario hacer un rediseño de la base de datos o **desnormalización**. A este proceso se le conoce como elaboración de una **tabla de hechos**, que involucra los siguientes elementos básicos.
* Identificación de los hechos
* Indentificación de las dimensiones
* Identificación de Jerarquías
* Identificación de niveles
* Identificación de atributos



![Definicio de hechos](http://shotcretemexico.com/cursos/base-datos/definicion_hechos.png)


###Caso de uso: Hechos ventas
En la siguiente imágen se puede observar de dónde surge el concepto de lo que se conoce como un **HECHO**
![Evento de hechos  ventas](http://shotcretemexico.com/cursos/base-datos/tabla_hechos_ventas.png)

###Actividad a entregar en archivo **sql**
Crear todas las tablas correspondientes al Hecho **ventas** a partir del diagrama siguiente
![Segundo entregable](http://shotcretemexico.com/cursos/base-datos/entregable2.png)

