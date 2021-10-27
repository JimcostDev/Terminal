# Terminal
Notas de comandos basicos para el manejo de una terminal linux
## Lista de comandos:

Comando/Sentencia | Concepto/Descripcion
--|--
```clear o Crtl + L``` | Limpiar pantalla de la terminal
```pwd``` | Ver en que directorio estoy ubicado (arbol de directorios)
```ls``` | Listar el contenido de un directorio
```ls --help``` | Ver opciones que me permite ```ls```
```ls -l``` | Mostrar un listado (ver mas información del directorio o archivo). La primer letra identifica el tipo de archivo ```(d = directorio, l = enlace, - = archivo)```, las demas letras ```(r, w, x)``` nos dice si el archivo tiene permiso de lectura (r), escritura (w) o ejecución (x)
```ls -l -h``` | Mostrar listado con detalles + el tamaño de una manera mas entendible
```alias``` | Ver listado de alias creados
```alias ls='ls -lh --color=auto'``` | Crear alias; es como una variable
```cd``` | Moverse entre directorios (cd = change directory) 
```cd .``` | Directorio actual
```cd ..``` | Devolverse un directorio 
```cd -``` | Devolverse al directorio inmediatamente anterior (a antes del ultimo cd que utilizamos)
```cd ~``` | Ir a mi directorio de usuario (home)
```cat``` | Ver el contenido de un archivo
```cat -n``` | Ver el contenido y me muestra el numero de lineas
```sudo (superuser do)``` | Convertirse en super administrador de manera temporal (root = usuario super administrador)
```sudo apt install nombre_app"``` | Instalar una aplicación (distribucion ubuntu, utliza el gestor de paquetes ```apt = Advanced Packaging Tool```
```touch hola_mundo.py``` | Crear un archivo totalmente vacio
```echo "hola" > prueba.txt``` | Crear un archivo con contenido, es este caso el archivo ```prueba.txt``` va a tener como contenido "hola"
```echo "como estas" >> prueba.txt``` | Agregar información al archivo ```prueba.txt``` va a tener como contenido "hola como estas"
```mkdir (make directory)``` | Crear un directorio; ```mkdir mi_directorio_1```
```mkdir -p proyecto/java/images``` | Crear el directorio "proyecto", dentro de este "java" y dentro de java, "images"
```cp (copy)``` | Copiar archivos ```cp origen destino``` = ```cp perfil.png ../../../proyecto/``` o ```cp index.html /c/workspace-jimcostdev/mi_directorio_1/proyecto/```
```cp -r``` | Copiar directorios (-r = recursivo) ```cp mi_directorio_1 mi_directorio_1_copia``` 
```rm (remove)``` | Eliminar archivos. ```rm nombre.ext```
```rm -i ``` | Eliminar el archivo, pero antes pregunta si deseo de verdad eliminarlo. ```rm -i nombre.ext```
```rm -r ``` | Eliminar directorios de manera recursiva ```rm -r directorio1```
```mv (move)``` | Mover archivos o directorios. ```mv nombre.ext carpeta/``` o ```mv directorio1/ /c/programas/```
```find``` | Buscar archivos ```find . -name *.png``` = Buscar (find) en la carpeta actual (.) todos(*) los archivos que sean .png (-name)

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
```GG``` | Ir al final
```dd``` | Cortar, con ```p``` se pega
```yy``` | Copiar, con ```p``` se pega
```x``` | Quitar un caracter a la derecha; esto sin estar en el modo insert
```X``` | Quitar un caracter a la izquierda; esto sin estar en el modo insert
```v``` | Entrar en modo visual (esto para seleccionar varias líneas)
```/+texto``` | Al pulsar «/» se abre la función de búsqueda. Entonces podremos escribir el texto que queremos buscar. El editor resaltará todas las apariciones de este texto. Pulsamos enter y nos llevará a la siguiente aparición de la búsqueda, con respecto a la posición de nuestro cursor
```n y N``` | Una vez realizada la búsqueda, el comando ```n``` nos lleva a la siguiente aparición de la cadena buscada. El comando ```N``` nos llevará a la anterior
```:%s/texto/texto_nuevo/g``` | Sustituir una palabra en todo el documento


