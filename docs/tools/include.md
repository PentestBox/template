Include Your own Tool
============================

There are many situations someone wants to run a tool which may be not be provided by [toolsmanager](https://docs.pentestbox.com/#tools-manager) or isn't installed by default in PentestBox. You can follow the guide below to include your own tool.

In order to include a tool in PentestBox, you need to do two things, download/clone tool files and then set alias for it. **alias** is basically a terminal command which need to be passed in PentestBox console, for example **sqlmap** is an alias for accessing SQLMAP.

Including a Python Based Tool
--------------------------------

* First download/clone the files of that tool in C:/PentestBox/bin/customtools
* Install any needed libraries using pip, for example if you need to install the **BeautifulSoup4** library then you can install it using **python -m pip install BeautifulSoup4**.
* Since python is preconfigured in PentestBox, you can run the tool by prepending **python** to the python file.
* To add an alias, open the **customaliases** file located in C:/PentestBox/bin/customtools/ folder.
* For example if you needed to add an alias for the sqlmap tool, then the alias for it would be `sqlmap=python "%pentestbox_ROOT%\bin\customtools\sqlmap\sqlmap.py" $*`
* Add the above line to customaliases and save the file
* Likewise you can create an alias for your tool. You can run your tool after restarting PentestBox.

Including a Ruby Based Tool
-------------------------------
* First download/clone the files of that tool in C:/PentestBox/bin/customtools
* Install any needed gems using gem, for example if you need to install the **nokogiri** library then you can install it using **gem install nokogiri**.
* Since ruby is preconfigured in PentestBox, you can run the tool by prepending **ruby** to the ruby file.
* For example if you needed to add an alias for the wpscan tool, then alias for it would be `wpscan=ruby "%pentestbox_ROOT%\bin\customtools\wpscan\wpscan.rb" $*`
* Add the above line to the customaliases and save the file
* Likewise you can create an alias for your tool. You can run your tool after restarting PentestBox.

Including an Executable Based Tool
-------------------------------
* First download/clone the files of that tool in C:/PentestBox/bin/customtools
* You can directly access the file by typing it's filename, for example you can access tool.exe by typing **tool.exe** on the console.
* For example, an alias for an executable would be like `tool="%pentestbox_ROOT%\bin\customtools\tool.exe" $*`.
* Add the above line to customaliases and save the file.
* Likewise you can create an alias for your tool. You can run your tool after restarting PentestBox.

Including a Java Based Tool
--------------------------------

* First download/clone the files of that tool in C:/PentestBox/bin/customtools
* Since Java is preconfigured in PentestBox, you can run the tool by prepending **java -jar** to the jar file.
* For example if you need to add an alias for "tool", then the alias for it would be `tool=start javaw -jar "%pentestbox_ROOT%\bin\customtools\tool.jar" $*`
* Add the above line to customaliases and save the file
* Likewise you can create an alias for your tool. You can run your tool after restarting PentestBox. 

You can have a look at the [aliases](https://github.com/PentestBox/configV2/blob/master/aliases) file for more examples of aliases.

