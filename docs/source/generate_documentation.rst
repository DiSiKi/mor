:github_url: https://github.com/JuLuSi/mor

**********************
Generate Documentation
**********************

Install Sphinx in the virtual environment
=========================================

Activate the `Firedrake <https://www.firedrakeproject.org/>`_ local environment
   
   .. code:: bash
	     
      source <path/to/your/firedrake/installation>/bin/activate
      
Install Sphinx and the RTD-Theme

   .. code:: bash

      pip install [--user] sphinx sphinx-rtd-theme

Make Documentation
==================

Make a local version of the documentation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can create a local Version of the documentation by adding/editing/deleting .rst-Files in the ``docs/sources/`` folder.

   #. Edit the ``docs/source/`` folder.

   #. Switch in the ``docs`` folder.

   #. Make documentation

      .. code:: bash

	 make html

   #. Congratulations your new documentation is ready! You can view it in your Browser by opening the file ``docs/build/html/index.html``.

   Feel free to create a pull request with your changes in the ``docs/source/`` folder.
   

Change the online documentation on `GithubIO <https://julusi.github.io/mor/>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  * If you have writing permission on https://github.com/JuLuSi/mor use the ``docs/gen-gh-pages.sh`` script:

    #. Push your changes in the ``docs/source/`` folder to the ``master`` branch.

    #. Execute the ``docs/gen-gh-pages.sh`` script: This script removes the old ``gh-pages`` branch and creates a new one using the ``docs/source/`` folder from the ``master`` branch.

  * Without writing permissions it is not possible to change the documentation on https://julusi.github.io/mor/ .
