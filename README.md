# Blog del Club Ajedrez Tomelloso

Este es el repositorio del Club Ajedrez Tomelloso. Se ha construído con [Hugo](https://gohugo.io/), un generador de páginas estáticas en Markdown. Se puede instalar siguiendo estos pasos: [Instalación de Hugo](https://gohugo.io/tutorials/installing-on-windows/)

Las reglas de como escribir Markdown y un editor que al escribir se actualiza su resultado lo podéis ver aquí: 
* [Reglas del Markdown](https://markdown.es/sintaxis-markdown/).
* [Editor online de Markdown](https://stackedit.io/editor#)

## Desarrollo

Para desarrollar en local se tiene que poner el comando:

```powershell

hugo server --theme=customchess

```

Y entonces la página se nos desplegará en la dirección: [http://localhost:1313](http://localhost:1313).

Tiene HMR, por lo que cualquier cambio en los Markdown es recargado en caliente.

# Despliegue

## Subir cambios de Git

Para realizar el despliegue lo primero que hay que hacer es dejar el repo actualizado. Para ello ejecutar el comando de git:

```powershell

git pull origin develop

```

Develop si es la rama que os queréis actualizar; sino el nombre de la rama que queráis actualizar.

Antes de publicar siempre tenéis que subir los cambios al repo. Para ello primero añadir los archivos con el comando de git desde la carpeta raíz:

```powershell

git add .

```

Después de añadir todos los archivos tenéis que hacer un commit con:

```powershell

git commit -m "Este es el mensaje del commit"

```

Cambiar el mensaje que sois capaces de dejarlo así. Por último teneis que hacer un push para que se actualice el repositorio remoto:

```powershell

git push origin develop

```

Develop si es la rama en la que estáis, sino el nombre de vuestra rama.


## Desplegar con Hugo

Para desplegar el código de Hugo hay que poner el comando:

```powershell

hugo --theme=customchess

```

Esto nos generará una carpeta public en la cual tendremos los ficheros HTML, Css y Javascript que podemos desplegar. De momento no tenemos despliegue automático por lo que si lo queremos desplegar en las página de github debemos actualizar el repo: [https://github.com/ajedreztomelloso/ajedreztomelloso.github.io](https://github.com/ajedreztomelloso/ajedreztomelloso.github.io) copiando y pegando a mano los ficheros.

Para desplegarlo en producción hay que generar un zip y subir los archivos en la carpeta /html con la opción Subir / Bajar Archivos.