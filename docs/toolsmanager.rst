Tools Manager
==========================

Tools Manager was introduced in PentestBox v2.0. Using this utility you can install/update/uninstall tools which are not there in PentestBox. This makes PentestBox more modular. The list of tools which can installed using toolsmanager can be found at `modules.pentestbox.com <https://modules.pentestbox.com>`_.

It is an interactive Installation utility, type **toolsmanager** on terminal to open it. First it will update itself from the Github Repository and then will display the menu. In case there is no internet connection, the script will wait for some time and then display the menu.

.. image:: https://i.imgur.com/DG7UfLC.png

You can see the list of tools by selecting a particular category. For example, if I choose the **Web Applications** category and press **10**, it will display something like this. At the time of writing, it only contains **whatweb**. 

.. image:: https://i.imgur.com/A8trOQm.png

Now if you want to install **whatweb**, then type **install whatweb** and it will install it. After installing, it will display the alias for the tool, in the case of whatweb it is **whatweb**.

.. image:: https://i.imgur.com/XoNT7Qh.png

.. note:: Since toolsmanager is just an installation utility, when any tool without re-distributable license is installed, the user automatically accepts the agreement provided by developer of that tool. 
