# Terminal/Shell 
Notas de comandos básicos para el manejo de una terminal Linux.
## Lista de comandos:

Comando/Sentencia | Concepto/Descripcion | Simulacón
--|--|--
```clear o Crtl + L``` | Limpiar pantalla de la terminal | [Ver imagen](https://user-images.githubusercontent.com/53100460/201367264-213d0ba9-e5a5-499d-9391-651aa8e733bf.PNG)
```pwd``` | Ver en que directorio estoy ubicado (arbol de directorios) | [Ver imagen](https://user-images.githubusercontent.com/53100460/201368146-d66c313a-4604-495e-9f37-b0a027066e17.PNG)
```ls``` | Listar el contenido de un directorio | [Ver imagen](https://user-images.githubusercontent.com/53100460/201369143-cd389462-b1b2-47bd-bc04-5a08d498e62b.PNG)
```ls --help``` | Ver opciones que me permite ```ls``` | 
```ls -l``` | Mostrar un listado (ver mas información del directorio o archivo). La primer letra identifica el tipo de archivo ```(d = directorio, l = enlace, - = archivo)```, las demas letras ```(r, w, x)``` nos dice si el archivo tiene permiso de lectura (r), escritura (w) o ejecución (x) | [Ver imagen](https://user-images.githubusercontent.com/53100460/201370028-146e2e0a-f7ff-48ab-a01d-543229907970.PNG)
```ls -l -h``` | Mostrar listado con detalles + el tamaño de una manera mas entendible | [Ver imagen](https://user-images.githubusercontent.com/53100460/201371125-621720a2-8709-461d-be3b-6af3765d8da7.PNG)
```alias``` | Ver listado de alias creados | [Ver imagen](https://user-images.githubusercontent.com/53100460/201372484-1af91ee3-c32a-4f62-a7f8-0e952d9e96c0.PNG)
```alias ls='ls -lh --color=auto'``` | Crear alias; es como una variable | [Ver imagen](https://user-images.githubusercontent.com/53100460/201373797-cd345dd3-a2c7-4cd9-bba7-c07a7b33546a.PNG)
```cd``` | Moverse entre directorios (cd = change directory) | 
```cd .``` | Directorio actual | 
```cd ..``` | Devolverse un directorio  | 
```cd -``` | Devolverse al directorio inmediatamente anterior (a antes del ultimo cd que utilizamos) | 
```cd ~``` | Ir a mi directorio de usuario (home) | 
```cat``` | Ver el contenido de un archivo | [Ver imagen](https://user-images.githubusercontent.com/53100460/201375670-dfef41b9-d8d5-4915-9340-137dabf2e739.PNG)
```cat -n``` | Ver el contenido y me muestra el numero de lineas | [Ver imagen](https://user-images.githubusercontent.com/53100460/201376317-a91a049e-5449-40b3-9b20-b40485f2a1ac.PNG)
```sudo (superuser do)``` | Convertirse en super administrador de manera temporal (root = usuario super administrador) | 
```sudo apt install nombre_app"``` | Instalar una aplicación (distribucion ubuntu, utliza el gestor de paquetes ```apt = Advanced Packaging Tool``` | 
```touch hola_mundo.py``` | Crear un archivo totalmente vacio | [Ver imagen](https://user-images.githubusercontent.com/53100460/201380239-091a3bb0-7ded-4b30-82f7-1270696a77ac.PNG)
```echo "hola" > prueba.txt``` | Crear un archivo con contenido, es este caso el archivo ```prueba.txt``` va a tener como contenido "hola" | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```echo "como estas" >> prueba.txt``` | Agregar información al archivo ```prueba.txt``` va a tener como contenido "hola como estas" | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```mkdir (make directory)``` | Crear un directorio; ```mkdir mi_directorio_1``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```mkdir -p proyecto/java/images``` | Crear el directorio "proyecto", dentro de este "java" y dentro de java, "images" | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```cp (copy)``` | Copiar archivos ```cp origen destino``` = ```cp perfil.png ../../../proyecto/``` o ```cp index.html /c/workspace- jimcostdev/mi_directorio_1/proyecto/``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```cp -r``` | Copiar directorios (-r = recursivo) ```cp mi_directorio_1 mi_directorio_1_copia``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```rm (remove)``` | Eliminar archivos. ```rm nombre.ext``` | [Ver imagen](https://user-images.githubusercontent.com/53100460/201380854-bb19ccbc-b28e-4a58-a1c9-d02f84928be7.PNG)
```rm -i ``` | Eliminar el archivo, pero antes pregunta si deseo de verdad eliminarlo. ```rm -i nombre.ext``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```rm -r ``` | Eliminar directorios de manera recursiva ```rm -r directorio1``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```mv (move)``` | Mover archivos o directorios. ```mv nombre.ext carpeta/``` o ```mv directorio1/ /c/programas/``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```find``` | Buscar archivos ```find . -name *.png``` = Buscar (find) en la carpeta actual (.) todos(*) los archivos que sean .png (-name) | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```find -iname``` | Obviar en la busqueda minusculas y mayusculas. ```find . -iname "prueba.txt"``` = Busca todos los archivos que tengan el nombre "prueba.txt" sin tener en cuenta Mayusculas y minusculas | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)
```find -type d``` | Buscar solo directorios ```find . -type d -iname "directorio"``` | [Ver imagen](https://www.jimcostdev.com/img/foto.jpeg)

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


