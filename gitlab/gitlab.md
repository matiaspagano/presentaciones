:title: GitLab
:author: Matías Pagano
:description: GitLab, administrador web de repositorios Git
:keywords: Gitlab
:css: gitlab.css

----

.. image:: images/gitlab_logo.png

----

Que es GitLab?
=============

GitLab es una aplicación opensource que nos permite administrar repositorios en git mediante una interfaz web.
Es un clon de <a href="http://github.com">GitHub</a> y es una herramienta muy potente para el desarrollo.

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

Inicializando el repsositorio Git de nuestro proyecto GitLab
============================================================
    
- En GitLab inicialmente tenemos un proyecto que no tiene un repositorio local asignado. 
- Tenemos dos opciones: , la primera opción se refiere a repositorios vacios y se muestran los pasos para 
	- Crear un repositorio vacío y enlazarlo al repositorio local de nuestro proyecto en GitLab.
	- Utilizar un repositorio ya creado y solo debemos asignarlo al proyecto de GitLab.
	
----

Pero... Antes que nada
======================

- GitLab utiliza claves SSH para permitir trabajar con los respositorios.
- Las claves SSH son utlizadas para establecer una conexión segura entre el sus repositorios y GitLab. 
- Con lo cual lo primero que necesitamos hacer es subir nuestra clave pública al proyecto.
- Si no realizamos esto el usuario no podrá subir los cambios realizado en su repositorio local al proyecto de GitLab!!

----

Generarando nuevas claves SSH:
==============================

Linux
-----

:code
	ssh-keygen -t rsa -C "your_email@example.com"

----

Generarando nuevas claves SSH:
==============================

Windows
-------

:code
	git-exe

----

Dudas?
======

