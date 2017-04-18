# PDAM-08
introducción a prototipos en iOS 

## Arquitectira de las aplicaciones de iOS
<img src="http://gabo.com.co/pdam/lab-8/lab-8-4.png" width="50%">

## Creación del proyecto
Para el desarrollo de aplicaciones en iOS, se recomienda usar XCode. Este IDE tiene todo lo necesario para manjear el desarrollo, assets y licencias de las aplicaciones.

* Abra XCode y seleccione la opción "Tabbed Application" que iniciará una aplicación base con un menu contextual.
<img src="http://gabo.com.co/pdam/lab-8/lab-8-5.png" width="50%">

* Para el nombre del proyecto utilice "pdam-08"
* Asegurese de seleccionar la opcion de "Swift" en el lenguaje
* Verifique que la aplicación este correctamente creada corriendo el emulador dando click al boton de play, el emulador es una aplicación aparte que se abrirá al terminar la compilación
<img src="http://gabo.com.co/pdam/lab-8/lab-8-2.png" width="50%">
* En XCode, abra el archivo "Main.storyboard", este archivo contiene la información del flujo de la interfaz de la aplicación. En el editor verá 3 vistas

** La vista que contiene los tabs
** La vista de la derecha
** La vista de la izquierda
<img src="http://gabo.com.co/pdam/lab-8/lab-8-6.png" width="50%">

* Agregue una tercera vista haciendo drag and drop de un elemento "ViewController", si no puede verlo use el siguiente icono para desplegar el menu lateral:
<img src="http://gabo.com.co/pdam/lab-8/lab-8-7.png" width="20%">

* Seleccione el "Tab Bar Controller", al seleccionar un elemento el menu lateral se activa con opciones para el elemento seleccionado. Ubique el menu de conexiones:
<img src="http://gabo.com.co/pdam/lab-8/lab-8-8.png" width="20%">

* Ubique el grupo de conexiones llamado "Triggered Segues", sobre el punto negro saldra un icono de +, arraste el icono hasta la tercera vista que se creó, esto hara que el controlador de tabs añada un nuevo tab referenciando a la nueva vista:
<img src="http://gabo.com.co/pdam/lab-8/lab-8-9.png" width="50%">


