# Terminal
Notas de comandos basico para el manejo de una terminal linux
## SQL (COMMAND LINE):

Comando/Sentencia | Concepto/Descripcion
--|--
```bash pwd``` | ver donde estoy ubicado (arbol de directorios)
```select * from cat``` | Visualizar el diccionario de datos del usuario con el que estoy conectado (catalogo)
```describe o desc name-table``` | visualizar estructura de la tabla
```set linesize 300``` | ancho cmd sql
```set pagesize 30``` | alto cmd sql
```BETWEEN``` | Entre un rango de valores
```NOT BETWEEN``` | No este entre un rango de valores
```IN``` | Selecciona de una lista
```NOT IN``` | Selecciona los valores que no estan en la lista
```IS NULL``` | Retorna valores nulos
```IS NOT NULL``` | Retorna valores No nulos
```LIKE``` | Busqueda de patrones 
```NOT LIKE``` | Retorna los que no cumplan con la busqueda de patrones
```ORDER BY```  | Se utiliza para ordenar, puedo ordernar asc-Ascendente(por defecto) desc-descendente
```NVL``` | Nivelar Valores Nulos a un numero
```JOIN``` | Poder seleccionar informacion de mas de una tabla
```UPPER ``` | Convertir a mayusculas. Ej: ```select ename, upper(ename) from emp;```
```LOWER ``` | Convertir a minusculas. Ej: ```select ename, lower(ename) from emp;```
```INITCAP``` | Convierte el Primer caracter en Mayuscula, el resto en minuscula. Ej: ```select ename, initcap(ename) from emp;```
```LPAD``` | Llenar o completar a la izquierda con. Ej: ```select ename, lpad(ename,10,'*') from emp;```
```RPAD ``` | Llenar o completar a la izquierda con. Ej: ```select ename, rpad(ename,10,'-') from emp;```
```LENGTH ``` | Retorna el tamano de una Cadena. Ej: ```select ename, length(ename) from emp;```
```SUBSTR ``` | Retorna una Subcadena. Ej: ```select ename, substr(ename, 1,3) from emp;```
```INSTR  ``` | Retorna la posicion del caracter dentro de la cadena. Ej: ```select ename, instr(ename,'A') from emp;```
