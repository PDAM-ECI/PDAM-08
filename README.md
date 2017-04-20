# PDAM-08
introducción a prototipos en iOS 

## Arquitectura de las aplicaciones de iOS
<img src="http://gabo.com.co/pdam/lab-8/lab-8-4.png" width="50%">

## Prototipo de una aplicación de iOS
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

* Añada un nuevo elemento de texto en la tercera vista, para esto arrastre un elemento "label" dentro de la tercera vista.

* En el menu lateral en la sección de atributos puede editar la terecera vista para ajustar el icono asignado, intente cambiar el icono y pruebe la aplicación nuevamente en el emulador.

* Repita el proceso pero esta vez añada una vista de navegación "Navigation Controller" para que sea la cuarta opcion del menu. Esto generara otra vista con un listado de opciones por defecto.
<img src="http://gabo.com.co/pdam/lab-8/lab-8-10.png" width="50%">

## Edición de código Swift para un listado de elementos

* Desde el menu izquierdo, cree un nuevo archivo Swift (ListViewController.swift) en la raíz de su proyecto, este archivo sera la logica de la vista de listado de elementos que se creo en el punto anterior.
<img src="http://gabo.com.co/pdam/lab-8/lab-8-11.png" width="50%">

Complete el código con el ejemplo de la imagen anterior para crear una clase que extienda de UITableViewController

* Desde el menu izquierdo, cree un nuevo archivo Swift (ListCell.swift) en la raíz de su proyecto, este archivo será la lógica de la fila del listado de elementos.

<img src="http://gabo.com.co/pdam/lab-8/lab-8-12.png" width="50%">

Complete el código con el ejemplo de la imagen anterior para crear una clase que extienda de UITableViewCell

* Desde la vista de history boar "Main.historyboard" seleccione la celda prototipo, en las opciones de la derecha vaya a a la opcion de Identity Inspector, en esta opcion ubique la casilla de class y dentro de ella escriba el nombre de la clase que creó en el punto anterior, esto asignará la logica a la vista seleccionada.

<img src="http://gabo.com.co/pdam/lab-8/lab-8-13.png" width="50%">

* Desde el mismo menu ubique la opcion de atributos y en la casilla de Identifier ponga el valor "listCell"
<img src="http://gabo.com.co/pdam/lab-8/lab-8-15.png" width="50%">

* De la misma manera, seleccionando el controlador del listado de elementos, haciendo click en el icono amarillo vincule la vista del controlador con la clase que creo anteriormente: ListViewController.swift

* Añada un elemento de tipo Label a la celda prototipo
<img src="http://gabo.com.co/pdam/lab-8/lab-8-14.png" width="50%">

* En la parte superior active la vista de edicion con asistente, esto mostrara dos ventanas para editar, a la derecha tendrá la vista de diseño y a la izquierda la vista de código. Asegurese que la ventana de la derecha muestre la clase "ListCell". Seleccione el label creado en el punto anterior y presionando la tecla "control" arrastre el mouse desde la vista de diseño hasta la vista de codigo como se muestra en el siguiente ejemplo.

Verifique que la variable que se crea al arrastrar el elemento sea un atributo de la clase, cuando XCode le solicite el nombre del componente use el siguiente: textUserLabel

El proceso anterior es la forma de vincular la vista con el controlador para poder controlar los componentes mediante el código.

<img src="https://media.giphy.com/media/l4FGtOsXaa4SdJbK8/giphy.gif" width="100%">

* Ahora añadirá el codigo como en el siguiente ejemplo para mostrar 5 filas con numeros
<img src="http://gabo.com.co/pdam/lab-8/lab-8-16.png" width="50%">

## Resultado final
<img src="https://media.giphy.com/media/l1KVbF3IGDNncqDzq/giphy.gif" width="50%">





