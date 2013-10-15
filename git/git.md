:title: Git
:author: Matías Pagano
:description: Tutorial Git
:keywords: Git
:css: git.css

----

.. image:: images/git.png

----

Que es Git?
===========

Git es un sistemas de control de versiones distribuido libre dieñado para manejar proyectos con velocidad y eficiencia.

.. image:: images/git-distributed.png
	:align: center

----

Características
=============== 

* Snapshots, no diferencias
* Casi todas las operaciones son locales
* Tiene integridad

----

Snapshots, no diferencias
=========================

* La mayoría de los demás sistemas almacenan la información como una lista de cambios en los archivos.
* Git modela sus datos más como un conjunto de instantáneas (snapshots) de un mini sistema de archivos.

----

Casi todas las operaciones son locales
======================================

* La mayoría de las operaciones en Git sólo necesitan archivos y recursos locales para operar.
* Para navegar por la historia del proyecto, Git no necesita buscarla en el servidor.

----

Tiene integridad
================

* Todo en Git es verificado mediante una suma de comprobación antes de ser almacenado, y es identificado a partir de ese momento mediante dicho checksum.
* Esto significa que es imposible cambiar los contenidos de cualquier archivo o directorio sin que Git lo sepa.

----

Instalación de GIT
==================

* Linux (Debian/Lihuen/Ubuntu)

.. code:: bash
		
	$ apt-get install git-core


* Linux (Fedora)
	
.. code:: bash
		
	$ yum install git-core

* Mac: http://code.google.com/p/git-osx-installer
* Windows: http://msysgit.github.com/
* Integrado con Eclipse (EGIT): http://www.eclipse.org/egit/
	
----

Obteniendo un repositorio git
=============================
    
- Inicializar un repositorio en un directorio existente

.. code:: bash

	$ git init

- Clonando un repositorio existente

.. code:: bash

	$ git clone gitlab@git.proyecto2013.linti.unlp.edu.ar/grupo.git
	
----

Directorio .git/
================

Cada repositorio Git es almacenado en la carpeta *.git* del directorio en el cual el repositorio ha sido creado.
Este directorio contiene la historia completa del repositorio. El archivo *.git/config* contiene la configuración local del repositorio.

----

Configuración del usuario
=========================

Configurá tu usuario e email para Git mediante los siguientes comandos:

.. code:: bash

	# Configura el usuario que será usado por git
	# Obviamente deberías usar tu nombre
	git config --global user.name "John Doe"
	# Lo mismo para el correo electrónico
	git config --global user.email "jdoe@example.com"

----

Operaciones Locales
===================

Git tiene tres estados principales en los que se pueden encontrar tus archivos: confirmado (committed), modificado (modified), y preparado (staged). 
 
.. image:: images/git-local-operations.png

----

Comprobando el estado
=====================

.. code:: bash

	$ git status
	# On branch master
	nothing to commit (working directory clean)

----

Creando contenido
=================

.. code:: bash

	# Creamos contenido
	# Agregamos todo (archivos y directorios) al repositorio
	$ git add .
	# Hacemos un commit al repositorio
	$ git commit -m "Initial commit"
	# Muestra el log (un historial)
	$ git log

----

Viendo las modificaciones
=========================

El comando *diff* de Git permite al usuario ver los cambios hechos. 

.. code:: bash

	# Mirá los cambios con el comando diff
	git diff
	# Comitea con -a sube los cambios de los archivos
	# pero no agrega automaticamente nuevos archivos
	git commit -a -m "Hay nuevos cambios"
    
----

Ciclo de vida de un archivo
===========================

.. image:: images/git-file-lifecycle.png
    :height: 600px
    :width: 800px

----

Repositorios Remotos
====================

- Son repositorios externos (ejemplo: de coworkers).
- Puede haber n remotos

----

El workflow completo
====================

.. image:: images/git-workflow.png
    :height: 600px
    :width: 800px

----

Conflictos
==========

Si al actualizar el repositorio local con el remoto (*git fetch* + *git merge* = *git pull*) no se puede realizar el merge por estar las mismas líneas modificada se produce un CONFLICTO. 

----

Conflictos
==========

Git nos avisa que debemos resolver nosotros el conflicto a mano:

.. code:: bash

	From git.proyecto2013.linti.unlp.edu.ar:ayudantes/grupo_777
	   2b33f0d..ea36b87  master     -> origin/master
	Auto-merging index.php
	CONFLICT (content): Merge conflict in index.php
	Automatic merge failed; fix conflicts and then commit the result.

----

Conflictos
==========

Debemos editar el archivo en conflicto que va a tener marcadas las lineas con problemas:

.. code:: bash

	<h1>
	<?php
	<<<<<<< HEAD
	print "hello Proyecto!!!"
	?>
	</h1>
	=======
	print "hello World!!!!!!!!!!"
	?>
	>>>>>>> ea36b870f9a0e1e6439758b6e681bd329a04db3d

y luego volverlo a agregar con *git add* y commiterarlo *git commit*.

----

Links:
======

* Git: http://git-scm.com/
* Libro: Pro Git: http://git-scm.com/book
* Git Cheatsheet: http://byte.kde.org/~zrusin/git/git-cheat-sheet-medium.png
* Git Cheatsheet Interactivo: http://ndpsoftware.com/git-cheatsheet.html

----

Dudas?
======

----


Fin
===

----

y recuerden...
==============

----

.. image:: images/git-windows-meme.jpg
