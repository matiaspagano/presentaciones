:title: GitLab
:author: Matías Pagano
:description: GitLab, administrador web de repositorios Git
:keywords: Gitlab
:css: gitlab.css

----

.. image:: images/gitlab_logo.png
	:alt: GitLab
	
----

Que es GitLab?
==============

GitLab es una aplicación opensource que nos permite administrar repositorios en git mediante una interfaz web.
Es un clon de http://github.com y es una herramienta muy potente para el desarrollo.

----

Antes que nada
======================

- GitLab utiliza claves SSH para permitir trabajar con los respositorios.
- Las claves SSH son utlizadas para establecer una conexión segura entre el sus repositorios y GitLab. 
- Con lo cual lo primero que necesitamos hacer es subir nuestra clave pública al proyecto.
- Si no realizamos esto el usuario no podrá subir los cambios realizado en su repositorio local al proyecto de GitLab!!

----

Generando nuevas claves SSH
===========================


.. code:: bash

	ssh-keygen -t rsa -C "your_email@example.com"

----

Agregando la clave SSH
======================

- Ir al perfil del usuario
- Agregar la clave pública (se va a utilzar en cada interacción con el servidor)
- Inicializar el repositorio Git de nuestro proyecto

----

Configurando el usuario del repositorio
=======================================

.. code:: bash

	git config --global user.name "Matías Pagano"
	git config --global user.email "matiasp@mail.linti.unlp.edu.ar"

----

Inicializando el repositorio Git de nuestro proyecto GitLab
============================================================
    
- En GitLab inicialmente tenemos un proyecto que no tiene un repositorio local asignado. 
- Tenemos dos opciones:
	- Crear un repositorio vacío y enlazarlo al repositorio local de nuestro proyecto en GitLab.
	- Utilizar un repositorio ya creado y solo debemos asignarlo al proyecto de GitLab.

----

Crear un repositorio vacío
==========================

Es la opción más común.

.. code:: bash

	mkdir grupo_1
	cd grupo_1
	git init
	touch README
	git add README
	git commit -m 'first commit'
	git remote add origin gitlab@git.proyecto2013.linti.unlp.edu.ar:/grupo_1.git
	git push -u origin master

----

Utilizando GitLab
=================

Teniendo nuestro respositorio git creado, podemos empezar a utilizarlo y en GitLab tener:

- El último estado de nuestros archivos. 
- Seguimiento de los *commits* realizados y las diferencias aplicadas.
- Una red con el crecimiento de las versiones y bifurcaciones que va tomando nuestro repositorio.
- Gráficos con estadísticas de uso.
- Creación y seguimiento de tareas (o *issues*) relativas al proyecto. 
- Una *wiki* con información propia de cada proyecto.

----


Dudas?
======

