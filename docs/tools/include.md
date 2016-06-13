Include Your own Tool
============================

There are many times a situation wants to run a tool which may be not be provided [toolsmanager](https://docs.pentestbox.com/#tools-manager) or not installed by default in PentestBox. You can follow the guide given below to include your own tool.

In order to include tool in PentestBox, you need to do two things, download/clone tool files and then set alias for it. **alias** is basically a terminal command which need to be passed in PentestBox console, for example **sqlmap** is an alias for accessing SQLMAP.

Including Python Based Tool
--------------------------------

* First download/clone files of that tool in C:/PentestBox/bin/customtools
* Install any needed libraries using pip, for example if you need to install **BeautifulSoup4** library then you can installing using **python -m pip install BeautifulSoup4**.
* As python is preconfigured in PentestBox, you can run tool by prepending **python** to the python file.
* To add an alias, open **customaliases** file located in C:/PentestBox/bin/customtools/ folder.
* For example if you needed to add alias for sqlmap tool, then alias for it would be **sqlmap=python "%pentestbox_ROOT%\bin\customtools\sqlmap\sqlmap.py" $*
* Likewise you can create alias for your tool and save the file. After your restart PentestBox change would be visible.

Including Ruby Based Tool
-------------------------------


Including Java Based Tool
-------------------------------

