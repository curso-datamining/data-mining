# Data Mining
Curso de Data Mining con Oracle 12c

##Entregable No.1
Instalación de Oracle 12c y de SQL Developer 4.1.x. Para ello sólo deberás de proporcionar las impresiones de pantalla de cada uno de los pasos de la instalación en un documento  de texto.
![Primer entregable](http://shotcretemexico.com/cursos/base-datos/entregable1.png)
##Entregable No. 2 y 3

###Introducción
El objetivo de la minería de datos es analizar los datos acumulados a lo largo de varios añosde operación de las empresas y buscar **relaciones y tendencias previamente desconocidas**. Esto es, hacer análisis de los datos a un nivel **táctico** y a un nivel **estrategico**.
Para ello es necesario primeramente preparar los datos para ese análisis (Datawarehousing), ya que las bases de datos normalizadas son bastante difíciles de manejar, sobre todo cuando se trata de hacer análisis estádisticos tanto inferenciales, como de tipo pronóstico (tendencias a futuro de la información de los datos).

Recuerda que la normalización es un proceso que debe de llevarse a cabo en la creacion de una base  de datos a un nivel **operativo** para garantizar la **integridad de datos**. Sin embargo al tratar de  analizar grandes cantidades de datos resulta muy ineficiente tener los datos en este tipo de formato, ya que el uso de **joins** para manejar multiples campos de distintas tablas se hace casi imposible o muy difícil de llevar a cabo.
Para resolver ese conflicto y poder hacer un análisis de datos (minería de datos) con las técnicas que veremos en este curso,  es necesario hacer un rediseño de la base de datos o **desnormalización**. A este proceso se le conoce como elaboración de una **tabla de hechos**, que involucra los siguientes elementos básicos.
* Identificación de los hechos
* Indentificación de las dimensiones
* Identificación de Jerarquías
* Identificación de niveles
* Identificación de atributos
* Formación de cubos y medidas



![Definicio de hechos](http://shotcretemexico.com/cursos/base-datos/definicion_hechos.png)


###Caso de uso: Hechos ventas
En la siguiente imágen se puede observar de dónde surge el concepto de lo que se conoce como un **HECHO**
![Evento de hechos  ventas](http://shotcretemexico.com/cursos/base-datos/tabla_hechos_ventas.png)

###Actividad a entregar en archivo **sql**
Crear todas las tablas correspondientes al Hecho **ventas** a partir del diagrama siguiente
![Segundo entregable](http://shotcretemexico.com/cursos/base-datos/entregable2.png)

##Entregable No. 4
###Intoducción
En este entregable vas a crear el usuario de  **Data Mining** a travéz del usuario de administración  **sys** y con la base de datos de conexion **pdborcl** que se generó automáticamente cuando instalaste oracle.
*1. Conectarse como administrador **sys** con el privilegio de **sysdba* y con el servicio de conexión **pdborcl**.
*2. Activar la base de datos de conexion con la linea ```sql ALTER PLUGGABLE DATABASE OPEN FORCE;```
*3. Una vez establecida la conexión crear al usuario **dmuser**. Es sumamente importante que le des ese nombre y como password igual usa **dmuser**, dale espacio de tablas **users** y en el temporal **tmp**,  otorgale el privilegio **connect**  y en cuotas **USERS**.
*4. Genera una conexión para **dmuser** usando la base de datos de conexion **pdborcl*
*5. Activar la opción de **Data Miner** y establecer una conexión con el recién creado **dmuser**. Autorizar que se instale las base de datos de muestra. Crear un nuevo Proyecto que se llame **Introduccion al análiis** generar un flujo de trabajo que se llame **Aseguradora parte 1**
*6. Agregar un neuvo origen de datos y verificar que este disponible el esquema de la aseguradora, el esquema de los carros y e esquema de datos en JSON.


