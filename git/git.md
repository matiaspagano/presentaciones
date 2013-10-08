:title: Git
:author: Matías Pagano
:description: Tutorial Git
:keywords: Git
:css: git.css

----

.. image:: images/git.png

---

Que es Git?
===========



----

Características
=============== 

* Snapshots, no diferencias
* Casi todas las operaciones son locales
* Tiene integridad

Second header
-------------

Third header
............

The drawback with reStructuredText is that you can't skip levels. You can't
go directly from level 1 to level 3 without having a level 2 in between.
If you do you get an error::

    Title level inconsistent

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

* Son repositorios externos (ejemplo: de coworkers).
* Puede haber n remotos

----

El workflow completo
====================

.. image:: images/git-workflow.png
    :height: 600px
    :width: 800px

----
Instalación de GIT
==================

* Linux 
	* Debian/Lihuen/Ubuntu :
		$ apt-get install git-core
	* Fedora:
		$ yum install git-core
* Mac:
	* http://code.google.com/p/git-osx-installer

* Windows:
	* http://msysgit.github.com/

* Integrado con Eclipse (EGIT):
	* http://www.eclipse.org/egit/
	
----

Más información:
================

* Git: http://git-scm.com/
* Libro: Pro Git: http://git-scm.com/book
* Git Cheatsheet: http://byte.kde.org/~zrusin/git/git-cheat-sheet-medium.png
* Git Cheatsheet Interactivo: http://ndpsoftware.com/git-cheatsheet.html

----

Dudas?
======
