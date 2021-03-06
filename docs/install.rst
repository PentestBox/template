Installation
==================

The PentestBox installation is very simple, first you need to `download <https://pentestbox.com/#download>`_ pentestbox. There are two versions of PentestBox:

* PentestBox without Metasploit
* PentestBox with Metasploit

.. note:: In order to use the PentestBox with Metasploit version, you will need to swtich off your antivirus and firewall before installation.

After downloading the file, you will be provided with a installer. Make sure the extraction path is ``C:/PentestBox/`` and then click next to
extract files.

After the extraction is finished, you can find PentestBox files in ``C:/PentestBox/``, you can start PentestBox using the **PentestBox.exe** or **PentestBox.bat** file.

Installation on a USB drive
-----------------------------

PentestBox is completely portable, that means you can carry it on a USB drive without losing any configuration. You can install PentestBox on a USB drive using the same installer file I mentioned above.

If your pendrive location is `F:` on your computer then you can change the installation path of the PentestBox installer from ``C:/PentestBox`` to ``F:/``. 

Sharing PentestBox over a Network
----------------------------------

Consider a environment where you want to use PentestBox on many computers like in your office, lab, etc. Instead of installing PentestBox on each and every computer, you can just install that on one computer and share that folder as a drive to other computers on the same network.

* First, right click on the PentestBox folder which is located in the C drive and select properties.

  .. image:: https://i.imgur.com/sBi2aF6.png
  
* Select the **Sharing** tab and then click on **Share**.

  .. image:: https://i.imgur.com/1h7BJ3x.png
  
* Change read permission to **read/write** and click Share.

  .. image:: https://i.imgur.com/PYxhhhI.png
  
* Now go the computer where you want to operate PentestBox and then click on Network and locate the PentestBox folder.
  
  .. image:: https://i.imgur.com/dnZj2oO.png
  
* Now go to my computer and then click on Map Network Drive.
  
  .. image:: https://i.imgur.com/m8SMKbv.png
  
* Enter the PentestBox path and click on Finish.
  
  .. image:: https://i.imgur.com/z3V2LpK.png
  
* Now that folder will be created as a Network Drive.
  
  .. image:: https://i.imgur.com/cwuMg3X.png
  
* Finally, you can use PentestBox like you are using on the installed computer.
  
  .. image:: https://i.imgur.com/1Zc4r6k.png

I have personally tested most of the tools on a shared PentestBox and they seem to be working absolutely fine. But if you face any issue with any tool inside the shared PentestBox, then please report it on the `forums <https://forum.pentestbox.com>`_ or send an e-mail to aditya@manifestsecurity.com
