# Departamentos y municipios de Colombia - Código SQL

Este repositorio contiene un archivo .sql que contiene la ingormación de la divicion politico administrativa de Colombia. La base de datos fue diseñada inicialmente utilizando la herramienta MySQL Workbench, luego alimendata utilizando archivos CVS por medio de phpMyAdmin.

## Información contenida en la base de datos

La información contenida en la base de datos corresponde a las 6 regiones de Colombia, los 32 departamentos mas el distrito de Bogota y las 1.123 entidades administrativas locales (municipios, áreas no municipalizadas y la isla de San Andrés).

## Origen de la información

Esta información es obtenida por el Departamento Administrativo Nacional de Estadística (DANE) y tiene por propietaria del conjunto de datos al Ministerio de Tecnologías de la Información y las Comunicaciones.

La información fue emitida el 17 de mayo de 2011 y al momento de consultar los datos actualizada el 20 de mayo de 2020.

Los datos fueron extraidos de la siguiente dirección web: https://www.datos.gov.co/Mapas-Nacionales/Departamentos-y-municipios-de-Colombia/xdk5-pm3f

## Información de las tablas

### Tabla regiones

La tabla regiones contiene 6 registros correspondiente a las regiones de Colombia según la información extraida del DANE. La estructura de la tabla corresponde a un campo id y al campo region que almacena el nombre de las regiones.

### Tabla departamentos

La tabla departamentos contiene 3 campos correspondites al id del departamento, nombre del departamento y el id de la region (que apunta a la tabla regiones). El id de los departamento no es autoincremental ni asignado automanticamente sino que corresponde al "Código DANE del departamento". Es por este motivo que los id no son susecivos. 

### Tabla municipios

Se debe aclarar primero que si bien el nombre de la tabla es municipios, esta contiene el registro de todas las entidades administrativas ocales del país. La tabla municipios contiene 3 campos correspondientes al id del municipio, nombre del minicipio y id del departamento (que apunta a la tabla departamentos). El id de la tabla municipios corresponde al al "Código DANE del municipio".
