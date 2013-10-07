:title: Git
:author: Matías Pagano
:description: Tutorial Git
:keywords: Git
:css: git.css

----

.. image:: images/git.png


Restructured text takes any line that is underlines with punctuation and
makes it into a heading. Each type of undeline will be made into a different
level of heading, but it is not the type that is important, but rather the
order of which each type will be enountered.

So in this presentation, lines underlined with equal (=) characters will be
made into a first-level (H1) heading.

----

First header
============

You can choose other punctuation characters as your level 1 heading if you like,
but this is the most common. Any if these character works::

    = - ` : ' " ~ ^ _ * + # < > .

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

Más información:
================

.. Git: http://git-scm.com/
.. Libro: Pro Git: http://git-scm.com/book
.. Git Cheatsheet: http://byte.kde.org/~zrusin/git/git-cheat-sheet-medium.png
.. Git Cheatsheet Interactivo: http://ndpsoftware.com/git-cheatsheet.html

----

Dudas?
======
