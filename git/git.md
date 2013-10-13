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



----

Características
=============== 

* Snapshots, no diferencias
* Casi todas las operaciones son locales
* Tiene integridad

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

Creando contenido
=================

.. code:: bash

	# Creamos contenido
	$ touch index.php
	$ mkdir css
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

¿Qué es un branch?
------------------

- Es un puntero a un commit

----

¿Y cómo sabe git en que branch estamos actualmente?
---------------------------------------------------

- Otro puntero: HEAD 

----

Branches
========

Cambiando de branch
-------------------

.. code:: bash

	$ git checkout testing

----

Trabajando con Branches
=======================

.. image:: images/git-branching-model.png
    :height: 550px
    
- http://nvie.com/posts/a-successful-git-branching-model/

----

Cambiando de branch
===================

.. code:: bash

	$ git checkout testing

![checkout](18333fig0306-tn.png)

* Lo único que hace es cambiar HEAD!

----

# Haciendo cambios en un branch

.. code:: bash

	$ vi index.php
	$ git commit -am 'made a change'


![changing-branches](18333fig0307-tn.png)

----

# Volviendo a master

.. code:: bash

	$ git checkout master

![master](18333fig0308-tn.png)

----

# Haciendo cambios en master

.. code:: bash

	$ vi index.php
	$ git commit -am 'made other changes'


![more-changes](18333fig0309-tn.png)

----

# Branching y merging

![first](18333fig0310-tn.png)

----

# Branching y merging

![second](18333fig0311-tn.png)

----

# Branching y merging

![third](18333fig0312-tn.png)

----

# Branching y merging

![fourth](18333fig0313-tn.png)

----

# Branching y merging: fast-forward

.. code:: bash

	$ git checkout master
	$ git merge hotfix

![fifth](18333fig0314-tn.png)

----

# Branching y merging

![sixth](18333fig0315-tn.png)

----

# Branching y merging: merge made by recursive

.. code:: bash

	$ git checkout master
	$ git merge iss53

![seventh](18333fig0316-tn.png)

----

# Branching y merging

![eighth](18333fig0317-tn.png)

----

# Merge: Conflictos

* Remotos

![remote](18333fig0322-tn.png)

----

# Merge: Conflictos

![remote-2](18333fig0323-tn.png)

----

# Merge: Conflictos

![remote-3](18333fig0324-tn.png)

----

Repositorios Remotos
====================

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
