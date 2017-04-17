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

Para desplegar el código de Hugo hay que poner el comando:

```powershell

hugo --theme=customchess

```

Esto nos generará una carpeta public en la cual tendremos los ficheros HTML, Css y Javascript que podemos desplegar. De momento no tenemos despliegue automático por lo que si lo queremos desplegar en las página de github debemos actualizar el repo: [https://github.com/ajedreztomelloso/ajedreztomelloso.github.io](https://github.com/ajedreztomelloso/ajedreztomelloso.github.io) copiando y pegando a mano los ficheros.

Para desplegarlo en producción hay que generar un zip y subir los archivos en la carpeta /html con la opción Subir / Bajar Archivos.