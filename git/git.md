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

Obteniendo un repositorio git
=============================
    
- Inicializar un repositorio en un directorio existente

.. code:: bash

	$ git init

- Clonando un repositorio existente

.. code:: bash

	$ git clone gitlab@git.proyecto2013.linti.unlp.edu.ar/grupo.git
	
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

Instalación de GIT
==================

* Linux Debian/Lihuen/Ubuntu :

.. code:: bash
		
	$ apt-get install git-core


* Linux Fedora :
	
.. code:: bash
		
	$ yum install git-core

* Mac: http://code.google.com/p/git-osx-installer
* Windows: http://msysgit.github.com/
* Integrado con Eclipse (EGIT): http://www.eclipse.org/egit/
	
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
