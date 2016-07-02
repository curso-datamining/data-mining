## Solucion tabla de hechos

```sql
CREATE TABLE PRODUCTO (ID_PRODUCTO INTEGER, 
DESCRIPCION VARCHAR2(120),  MARCA VARCHAR2(120), 
CATEGORIA VARCHAR2(80), PRECIO FLOAT,
CONSTRAINT PK_ID_PRODUCTO PRIMARY KEY (ID_PRODUCTO));

CREATE TABLE FECHA (ID_FECHA INTEGER, DIA INTEGER,  MES INTEGER, 
ANIO INTEGER,
CONSTRAINT PK1_ID_FECHA PRIMARY KEY (ID_FECHA));

CREATE TABLE ALMACEN (ID_ALMACEN INTEGER, NUMERO INTEGER,  
NOMBRE VARCHAR2(120), ESTADO VARCHAR2(80), MUNICIPIO VARCHAR2(80),
CONSTRAINT PK2_ID_ALAMACEN PRIMARY KEY (ID_ALMACEN));

CREATE TABLE CAJERO (ID_CAJERO INTEGER, NOMBRE VARCHAR2(80), 
A_PATERNO VARCHAR2(80), A_MATERNO VARCHAR2(80), SUELDO FLOAT,
CONSTRAINT PK3_ID_CAJERO PRIMARY KEY (ID_CAJERO));
```