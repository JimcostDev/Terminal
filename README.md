# Terminal
Notas de comandos basicos para el manejo de una terminal linux
## Lista de comandos:

Comando/Sentencia | Concepto/Descripcion
--|--
```pwd``` | ver en que directorio estoy ubicado (arbol de directorios)
```ls``` | listar el contenido de un directorio


## Editor VIM:
Comando/Sentencia | Concepto/Descripcion
--|--
```i``` | Modo  inserción (--INSERT--)
```:w``` | Permite guardar el fichero
```:q``` | Salir de Vim. Si el fichero ha sido modificado pero no se ha guardado, nos advertirá y no podremos salir de Vim usando este comando
```:q!``` | Salir de Vim, descartando posibles cambios no guardados que se hayan realizado en el fichero
```:wq``` | Hace el guardado del archivo y después sale de Vim
```u``` | deshacer cambios, es como un ctrl + z
```Ctrl+r``` | Rehacer una acción
```$``` | Ir al final de la línea
```0``` | Ir al principio de la línea
```gg``` | Ir al inicio
```gg``` | Ir al final
```dd``` | Cortar, con ```p``` se pega
```yy``` | Copiar, con ```p``` se pega
```x``` | Quitar un caracter a la derecha; esto sin estar en el modo insert
```X``` | Quitar un caracter a la izquierda; esto sin estar en el modo insert
```v``` | Entrar en modo visual (esto para seleccionar varias líneas)
```/+texto``` | Al pulsar «/» se abre la función de búsqueda. Entonces podremos escribir el texto que queremos buscar. El editor resaltará todas las apariciones de este texto. Pulsamos enter y nos llevará a la siguiente aparición de la búsqueda, con respecto a la posición de nuestro cursor
```n y N``` | Una vez realizada la búsqueda, el comando ```n``` nos lleva a la siguiente aparición de la cadena buscada. El comando ```N``` nos llevará a la anterior
```:%s/texto/texto_nuevo/g``` | Sustituir una palabra en todo el documento


```bash 
	pw
```

```shell 
	cd directorio1
```
