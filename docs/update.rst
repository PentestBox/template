Update Feature
===================

Maintaining a product is always much more important than actually making one. That is why to keep all the tools updated inside PentestBox we have included an update utility. Also I have added ``update config`` which will be used as a medium to fix the bugs if any comes up.
You would see something similar if you typed ``update`` on console.

.. image:: https://i.imgur.com/Ea1WWDF.png

It will first update itself from it's Github Repository if there are any changes and then display the menu. In case there is no internet connection, the script will wait for some time and then display the menu.

For example if you need to update your **Web Aplications Tools** then just type **update webapplication**, you can update all the tools with one command by typing **update all**.

How does the update feature work in the backend ?
-------------------------------------------
PentestBox is an open source project, so all files that are used in PentestBox are there on it's `Github Repositories <https://github.com/pentestbox>`_ . 

You can find it's update script `here <https://github.com/pentestbox/scripts/blob/master/update.py>`_ . Nearly 80% of the tools which are shipped in PentestBox are fetched from their respective Github repositories, other are provided in zip format or in other way which are then manually configured in PentestBox. 

Whenever you type **update** on console, you will see it trying to update something, at the moment it is updating itself. Then whenever you provide a command to update a set of tools, for example ``update webapplication``, it will try to update the tools which are located in ``C:/PentestBox/bin/webapplications/``, as most of the tools are based on git VCS, it requires less data to acquire the changes of the respective tool.
