Installation
============

The first thing to do is to clone the repository with the project

.. code-block:: console

    $ git clone https://github.com/AlbertoCanoD/TFG

Then we must consider whether we are running a Linux distribution or a Windows system.

- In the case of using a Windows, we must install the "requeriments-windows.txt" which
  excludes "ssdeep" and "py-tlsh". In addition "python-magic-bin" is installed.

.. code-block:: console

    $ pip install -r requeriments-windows.txt

- In the case of using a Linux distribution, the "requeriments.txt" must be installed,
  and ssdeep must be installed later.

.. code-block:: console

    $ pip install -r requeriments.txt
    $ sudo apt install build-essential libffi-dev libfuzzy-dev
    $ BUILD_LIB=1 pip install ssdeep