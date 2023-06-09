# Redirección de salida estándar (stdout):

- ">" redirige la salida de un comando hacia un archivo, sobrescribiendo su contenido si el archivo ya existe.

## Ejemplo:

### ls > archivos.txt 
Escribirá la lista de archivos y directorios en el archivo "archivos.txt".

- ">>" redirige la salida de un comando hacia un archivo, pero agrega al final del archivo en lugar de sobrescribirlo.

## Ejemplo:

### echo "Hola" >> saludo.txt
Agregará la cadena "Hola" al final del archivo "saludo.txt".

- "&>" redirige tanto la salida estándar como la salida de error hacia un archivo.

## Ejemplo:

### comando &> registro.txt 
redirigirá tanto la salida estándar como la salida de error del comando hacia el archivo "registro.txt".

# Redirección de entrada estándar (stdin):

- "<" redirige la entrada de un comando desde un archivo en lugar del teclado.

## Ejemplo: sort < numeros.txt 
Ordenará los números contenidos en el archivo "numeros.txt".

- "|" (pipe) redirige la salida de un comando hacia la entrada de otro comando.

## Ejemplo: ls | grep ".txt" 
Lista los archivos en el directorio actual y pasa la salida a través de grep para encontrar los archivos que contengan ".txt".

# Redirección de salida de error estándar (stderr):

- "2>" redirige la salida de error de un comando hacia un archivo.

## Ejemplo: comando_inexistente 2> error.txt 
Redirigirá los mensajes de error generados por el comando comando_inexistente hacia el archivo "error.txt".

- "2>>" redirige la salida de error de un comando hacia un archivo, pero agrega al final del archivo en lugar de sobrescribirlo.

## Ejemplo: comando_inexistente 2>> errores.txt
Agregará los mensajes de error generados por el comando comando_inexistente al final del archivo "errores.txt".

- "2>&1" redirige la salida de error hacia la salida estándar.

## Ejemplo: comando 2>&1 
Redirigirá la salida de error del comando hacia la salida estándar.

