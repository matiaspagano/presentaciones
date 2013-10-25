:title: Trabajos Cursada proyecto de Software 2013
:author: Matías Pagano
:description: Trabajos Cursada proyecto de Software 2013
:keywords: Trabajos Cursada proyecto de Software 2013
:css: trabajos_proyecto2013.css

----

Trabajos Proyecto de Software 2013
==================================
	
----

Cooperativa MercoFlor
=====================

Objetivo del trabajo:
---------------------

Se desea realizar un software de gestión para una cooperativa comercializadora de flores.
El modo de trabajo que tiene se basa en un catálogo de especies de flores, con un stock, y
socios que llevan cierta cantidad de ejemplares de ciertas especies, y clientes que las compran.
Se desea llevar un control sobre las operaciones que se realizan en la cooperativa, así como
también listados y estadísticas.


----

Cooperativa MercoFlor
=====================

Objetivo del trabajo:
---------------------

Se desea realizar un software de gestión para una cooperativa comercializadora de flores.
El modo de trabajo que tiene se basa en un catálogo de especies de flores, con un stock, y
socios que llevan cierta cantidad de ejemplares de ciertas especies, y clientes que las compran.
Se desea llevar un control sobre las operaciones que se realizan en la cooperativa, así como
también listados y estadísticas.

Destinatarios:
--------------
El personal de la cooperativa (administración y gestión del sistema), los socios de la misma
(solo reportes). 

----

Cooperativa MercoFlor
=====================

Especificacion:
---------------

El sistema debe contar con ciertos módulos que permitan dicha gestión.

En esta primera etapa, será necesaria la implementación de los siguientes módulos:

- Módulo de clientes (quienes compran)

- Módulo de socios (quienes entran mercadería)

- Módulo de inquilinos (entran mercadería pero no son socios, solo alquilan un espacio para comercializar)

- Módulo de especies (ABM de especies)

- Módulo de Ingreso (gestión de ingreso de mercadería al predio)

----


Cooperativa MercoFlor
=====================

Módulo de clientes, socios e inquilinos:
----------------------------------------

Estos módulos deben permitir realizar ABM de clientes, socios e inquilinos. 

- Manejan los siguientes datos comunes: Nombre y Apellido, CUIT, dirección de E­mail, Dirección, Razón Social.

- Cada uno podrá registrar hasta dos ayudantes; de los cuales se conoce el Nombre y Apellido, y su DNI.

- Se debe obtener el mapa de zonificación de los mismos en Google Maps (cuyas coordenadas también están contenidas en dichos datos).

----

Cooperativa MercoFlor
=====================

Módulo de Ingreso:
------------------

- Este módulo permitirá realizar ABM de plantas/flores ingresadas por socios e inquilinos. 

- La información que se debe registrar por cada socio o inquilino que ingresa al predio es: Socio/Inquilino, Fecha y Hora de Ingreso. 

- Un socio o inquilino podrá ingresar una o mas especie de planta o flores. Por cada una de ella deberá registrarse la siguiente información: Especie a la que pertenecen, color, cantidad disponible, precio.

----

Cooperativa MercoFlor
=====================

Módulo de Especies:
-------------------

- Este módulo permitirá realizar ABM de especies. 

- La información que se debe registrar es: Nombre vulgar de la especie, nombre científico, hábitat, región, época del año en que florece, tipo de especie(Flor, Verde, etc)

----

Cooperativa MercoFlor
=====================

Alcance:
--------

- Se debe tener un Frontend y un Backend;

- Frontend se refiere a la parte pública, en donde se ven los listados de plantas por especie con su stock.

- Backend es la parte de administración, la cual va a requerir login (socios y administrador), y dependiendo del tipo de usuario, son las acciones que se tendrán disponibles. En este último, se dan de alta las especies, los socios y las plantas (también se modifican y/o eliminan, además de tener el listado de cada uno).

- De momento, el alta de Socios, Inquilinos y Clientes será hecho por un único usuario.

----

Dudas?
======

----

Fundación Bioquímica Argentina (FBA)
====================================

Objetivo del trabajo:
---------------------

- A pedido de la Fundación Bioquímica Argentina (FBA) se va a implementar un soft que permita realizar un seguimiento de controles de calidad de distintos laboratorios de Latinoamérica en el marco del Programa de Evaluación Externa de Pesquisa Neonatal (PEEC).

- Estos controles se basan en pruebas (denominadas encuestas) que se realizan en forma bimensual por los laboratorios participantes y cuyos resultados son enviados y analizados desde la FBA para establecer el grado de certeza alcanzado (estableciendo de esta manera un control de calidad sobre los mismos).

----

FBA
===

Especificación:
---------------

- La FBA envía en forma bimensual una encuesta (compuesta por dos pruebas) a distintos laboratorios.  Cada encuesta,que ya fue analizada previamente y cuenta  con un resultado exacto proporcionado por la FBA, se conforma de dos muestras de sangre  enviadas por correo postal a los laboratorios. Los laboratorios realizan las pruebas correspondientes y luego deben informar sus propios resultados al sistema.

- Tanto los laboratorios participantes como  el personal interviniente de la FBA tendrán un usuario en el sistema. Estos usuarios serán gestionados por un usuario administrador quien es el único que podrá dar de baja efectiva cualquier información cargada.

----

FBA
===

Especificación:
---------------

El sistema además, debe contar con ciertos módulos que permitan la gestión de las pruebas,el seguimiento de las mismas y la generación de algunos reportes.

En esta primera etapa, será necesaria la implementación de los siguientes módulos:

- Módulo de gestión de usuarios

- Módulo de gestión de encuestas

- Módulo de gestión de los laboratorios participantes

- Módulo para el ingreso de los datos de referencia para las pruebas:  tipos de pruebas, métodos, reactivos, calibradores y papel de filtro e interpretación y decisión

- Módulo para la carga de resultados

----

FBA
===

Módulo de gestión de usuarios:
------------------------------

El sistema deberá contemplar tres roles de usuarios:

- Administrador: quien gestionará los restantes usuarios del sistema y la información de referencia (datos relacionados a las pruebas)

- Personal de la FBA: quienes serán los encargados de habilitar una encuesta y acceder todos los informes

- Laboratorios: quienes podrán cargar los resultados de cada encuesta y visualizar su informe particular y aquellos que sean de dominio público.

----

FBA
===

Módulo de Gestión de Encuestas: 
-------------------------------

Este módulo permitirá gestionar la información de cada encuesta. La misma deberá contemplar:

- Fecha de inicio

- Fecha de fin

- Resultados correspondiente las dos muestras de la encuesta.

Este módulo  estará disponible únicamente para el personal de la FBA.

----

FBA
===

Módulo de Laboratorios
----------------------

Alta de Laboratorios: Esta opción estará disponible únicamente por el  el personal de la FBA. 

- Datos: Número secuencial de ingreso al programa, Código de Laboratorio, Institución, Sector, Responsable, Domicilio, Domicilio para el envío de la correspondencia, Ciudad, País, Código postal, Correo electrónico, Teléfono/Fax, Fecha de ingreso, Tipo de Laboratorio, Empresa a través de la cual se inscribe

- Además: Prueba para la cual se inscribe (estas pruebas se denominan analitos y se cargan desde una tabla de referencia. Sus valores iniciales son: Phe/TSH/IRT/Gal/Otro

Sería importante obtener el mapa de zonificación de los laboratorios en Google Maps.

----

FBA
===

Módulo de Laboratorios
----------------------


Baja de Laboratorios: Como se quiere llevar un seguimiento histórico de las pruebas, para dar de baja un laboratorio, tendremos dos opciones:

- una opción donde el laboratorio pasa a estado inactivo guardando la fecha de baja.

- una opción donde efectivamente se elimine la información de los laboratorios del sistema en forma definitiva (disponible sólo para el administrador del sistema).

----

FBA
===

Módulo para el ingreso de los datos de referencia
-------------------------------------------------

Cada prueba tiene asociado distintos atributos. 
Los datos a tener en cuenta son:  tipos de pruebas, métodos,  reactivos, Calibradores  y Papel de filtro e  Interpretación y Decisión

----

FBA
===

Módulo de Gestión de los Resultados
-----------------------------------

Los resultados de las pruebas (encuestas) serán ingresados por cada laboratorio. 

Para el ingreso de los resultados se deberán tener en cuenta:

- Fecha de recepción del material remitido por el PEEC (Fecha de recepción)

- Fecha de análisis

- Fecha de ingreso de los resultados al PEEC (Fecha de ingreso)

- Para cada analito (prueba dentro de la encuesta) se deberán poder ingresar los códigos correspondientes y los resultados

----

Dudas?
======

-----

Condiciones generales
=====================

- Debe ser desarrollado utilizando PHP, HTML5, CSS3 y MySql respetando el modelo en capas MVC.

- Pueden utilizar PDO como mecanismo de abstracción de bases de datos. 

- Debe tener en cuenta los conceptos de Semántica Web proporcionada por HTML5 siempre y cuando sea posible con una correcta utilización de las etiquetas del lenguaje.

- El trabajo será evaluado desde el servidor de la cátedra que cada grupo deberá gestionar mediante Git. No se aceptará ninguna entrega que no esté en tiempo y forma en el servidor provisto por la cátedra.

- El ayudante a cargo evaluará el progreso y la participación de cada integrante mediante las consultas presenciales y el seguimiento mediante GitLab.

- Toda vista (HTML5 y CSS3) debe validar contra las especificaciones corrientes de la W3C (http://validator.w3.org/). Se puede utilizar jQuery.

----

Mas Dudas?
==========
