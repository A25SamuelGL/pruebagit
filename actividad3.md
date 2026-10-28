# Guía básica de comandos de Linux
## Introducción
**Linux** es un sistema operativo muy utilizado en **servidores, ordenadores y dispositivos**. Una de sus *principales características* es la posibilidad de administrar el sistema mediante una terminal.

En esta guía aprenderás algunos de los ***comandos básicos de Linux*** para moverte por el sistema de archivos, crear y eliminar archivos y carpetas, y consultar información.

### Objetivo: Aprender los comandos esenciales para comenzar a trabajar con la terminal de Linux.

### Abrir la terminal
Para utilizar los comandos debemos abrir una terminal.

En **Ubuntu** podemos hacerlo mediante el menú de aplicaciones o utilizando el atajo:
```bash
Ctrl + Alt + T
```
Una vez abierta, aparecerá una línea similar a:

![alt text](../actividad2/imagenes/image.png)

***El símbolo $ indica que podemos introducir un comando.***

## Comandos básicos
 ### pwd

**Muestra la ubicación de la carpeta en la que nos encontramos.**

**Ejemplo de resultado `pwd`:**

![alt text](../actividad2/imagenes/image1.png)

### ls

**Muestra los archivos y carpetas del directorio actual.**


También podemos utilizar opciones para obtener más información:

`ls -l`

Para mostrar también los archivos ocultos:

`ls -la`

**Ejemplo :**

![alt text](../actividad2/imagenes/image2.png)

### cd
**Permite cambiar de directorio.**

Por ejemplo, para entrar en una carpeta llamada **Scripts**:

`cd Scripts`

Para volver a la carpeta anterior:

`cd ..`

Para volver directamente a la carpeta personal:

`cd ~`

**Ejemplo :**

![alt text](../actividad2/imagenes/image3.png)

### mkdir
**Sirve para crear una carpeta.**

`mkdir proyectos`

**Esto creará una carpeta llamada proyectos.**

### touch
**Permite crear un archivo vacío.**
```
touch ejemplo.txt
```
Después podemos comprobar que se ha creado utilizando:

`ls`

### cp
**Se utiliza para copiar archivos o carpetas.**

Por ejemplo:
```
cp ejemplo.txt copia.txt
```
**Este comando crea una copia de ejemplo.txt llamada copia.txt.**

### mv
**Permite mover o cambiar el nombre de un archivo.**

Para cambiar el nombre:
```
mv ejemplo.txt documento.txt
```
Para moverlo a otra carpeta:
```
mv documento.txt Documentos/
```
### rm
**Sirve para eliminar archivos.**
```
rm documento.txt
```
***⚠️ Precaución: los archivos eliminados mediante rm normalmente no pasan por la papelera de reciclaje. Utiliza este comando con cuidado.***

**Para eliminar una carpeta vacía:**
```
rmdir proyectos
```
### cat
**Muestra el contenido de un archivo de texto.**
```
cat documento.txt
```
*Es especialmente útil para consultar rápidamente archivos pequeños.*

### clear
**Limpia el contenido visible de la terminal.**

`clear`

*Los comandos introducidos anteriormente no se eliminan del historial; simplemente dejan de aparecer en pantalla.*

## Resumen de comandos

| Comando | ¿Para qué sirve? | Ejemplo |
|---|---|---|
| `pwd` | *Saber en qué directorio estás* | `pwd` |
| `ls` | *Ver archivos y carpetas* | `ls` |
| `cd` | *Entrar en otra carpeta* | `cd Documentos` |
| `mkdir` | *Crear una carpeta nueva* | `mkdir Fotos` |
| `touch` | *Crear un archivo vacío* | `touch notas.txt` |
| `cp` | *Copiar archivos o carpetas* | `cp archivo.txt copia.txt` |
| `mv` | *Mover o cambiar el nombre* | `mv viejo.txt nuevo.txt` |
| `rm` | *Borrar un archivo* | `rm notas.txt` |
| `cat` | *Ver lo que contiene un archivo* | `cat notas.txt` |
| `clear` | *Limpiar la terminal* | `clear` |


### Ejemplo práctico
**A continuación, vamos a utilizar varios comandos para crear una pequeña estructura de archivos.**

*Primero creamos una carpeta llamada practica:*
```
mkdir practica
```
Entramos en ella:
```
cd practica
```
Creamos un archivo:
```
touch notas.txt
```
Comprobamos que existe:
```
ls
```
Creamos una copia:
```
cp notas.txt copia.txt
```
Finalmente, comprobamos el contenido de la carpeta:
```
ls -l
```
**El resultado debería ser este:**

![alt text](../actividad2/imagenes/image4.png)

## Consejos de seguridad
Antes de ejecutar un comando en Linux, es importante saber qué acción realizará.

Comprueba siempre el nombre del archivo antes de utilizar rm.

Ten cuidado con los comandos ejecutados con sudo.

No ejecutes comandos que no comprendas.

Realiza copias de seguridad de los archivos importantes.

**Recuerda que Linux distingue entre mayúsculas y minúsculas.**

Por ejemplo:

***Documento.txt***

y

***documento.txt***

son dos archivos diferentes.

## Conclusión
>Los comandos de Linux permiten realizar muchas tareas de administración y gestión de archivos desde la terminal. Los comandos vistos en esta guía constituyen una base para comenzar a trabajar con un sistema Linux.

> Una vez dominados estos comandos, se pueden aprender otros relacionados con la gestión de usuarios, permisos, redes, procesos y administración del sistema.

**Comandos principales aprendidos**
* pwd
* ls
* cd
* mkdir
* touch
* cp
* mv
* rm
* cat
* clear

## Recursos
**Para seguir aprendiendo sobre Linux, puedes consultar:**

[Ubuntu Documentation](https://help.ubuntu.com/)

[Linux man-pages](https://linux.die.net/man/)

[GNU Coreutils](https://www.gnu.org/software/coreutils/)

## Mas comandos


## Información del proyecto

Esta documentación se ha elaborado utilizando Markdown.
El control de versiones se realiza mediante Git
y el repositorio remoto se encuentra alojado en GitHub.

 ## Próximas mejoras.
Añadir mas información mas detallada de los comandos
Añadir mas comandos de Linux
Estructurar a la perfección el proyecto
