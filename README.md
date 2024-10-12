##Proyecto de Ejemplo
En este proyecto practicaremos mediante la técnica de gitFlow
y de manera manual a interactuar entre distintos usuarios con
proyecto basado en la enseñanza de JavaScript y la documentación
correspondiente.

Documentación del Proceso de Desarrollo Usando Git Flow

####1. Introducción a Git Flow
   Git Flow es una metodología de ramificación en Git que permite gestionar el desarrollo de software de manera organizada y efectiva. Fue propuesta por Vincent Driessen en 2010 y se basa en el uso de ramas específicas para el desarrollo, las características, los lanzamientos y los arreglos de errores.

##Importancia de Git Flow
#-Organización: Proporciona una estructura clara para el manejo de diferentes etapas del desarrollo.
#-Colaboración: Facilita el trabajo en equipo al permitir que múltiples desarrolladores trabajen en diferentes características de forma simultánea sin interferencias.
#-Control de Versiones: Permite un control de versiones más preciso al separar el desarrollo de nuevas características y la preparación de lanzamientos.
-Mejor Gestión de Errores: Los hotfixes permiten corregir rápidamente errores críticos en producción sin afectar el desarrollo en curso.

####2. Descripción del Proceso Realizado
        ## USUARIO1
   #-Se ha iniciado por el usuario1 la carpeta del proyecto y se ha encargado de crear el repositorio y la estructura inicial de archivos y el contenido consistente en la cabecera, la barra de navegación y acceso al HOME,Así como el footer. Haciendo una pequeña descripcion en el cuerpo del HTML de ejemplos practicos de JavaScript
   Se ha usado mkdir despliegue-practica, git init para iniciar el repositorio, inicialmente mediante touch hemos creado los archivos de index, styles y script para cumplimentarlos a continuación, así como el documento README.md, en el que ahora estamos, a traves de code, hemos cumplimentado el código necesario, en HTML y CSS para la estructura inicial requerida.
   #-Posteriormente a crearlo, hemos hecho los pertinentes add, commit y hemos enlazado con nuestra cuenta de github mediante remote add origin
   Depues lo hemos empujado con push -u origin main

#- Hemos iniciado y configurado el flow con git flow init
- Creamos con el usuario1 feature start mejora-navegacion, para completar aspectos de la estructura inicial que habiamos pasado por alto
#- Se ha vuelto hacer el respectivo add, commit y cerramos este feature finish mejora-navegacion
Esto nos devuelve a la rama develop (en proceso de desarrollo)
        ##USUARIO 2
#Es el encargado del contenido HTML y de los atributos  
crearmos la rama feature start contenidoHTML   
modificamos y agregamos el contenido en javaScript y HTML
y hacemos los pasos pertinentes para hacer el commit y cerrar la rama.
#Iniciamos una segunda rama con el usuario2 , y creamos el ejemplo de los atributos y repetimos el mismo proceso que anteriormente y cerramos la rama mediante git flow feature finish atributosHTML  
Una vez hecho esto y estar en develop lo empujamos al repositorio remoto 
       ##USUARIO 3
#El usuario3 es el encargado del estilo y creará un ejemplo de modificar estilos mediante javascript, una vez hecho esto, codificando lo necesario volveremos a repetir el proceso para elcommit, la finalización de la rama y empujar al repositorio remoto.
Al mismo tiempo el usuario 3 crea un release y su etiquetado, en este punto hemos tenido problemas y lo hemos hecho manualmente.

            ##USUARIO 1
Por último el usuario 1 hace un hotfix sobre el contenido del usuario 2. Para ello usamos el comando  git flow hotfix start mejorasV_1_0, y el proceso restante es el mismo que los pasos anteriores para hacer commit, terminar la rama y empujar al repositorio remoto, otra vez hemos tenido problemas con el etiquetado y lo hemos vuelto a completar manualmente
