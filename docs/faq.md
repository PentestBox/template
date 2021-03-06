Frequently Asked Questions
==============================

When will it be available for Linux/Mac?
------------------------------------------

PentestBox was developed to provide the best pentetration testing environment for Windows users. So it will never be developed for Linux/Mac. For Linux/Mac you can use any Linux Pentesting Distro.

How can I work in FullScreen in PentestBox?
----------------------------------------------

Just press Alt + Enter while using PentestBox to go into FullScreen Mode and do the same to come back in normal mode.

Why is [ToolName] not working in PentestBox?
-----------------------------------------------

In case if you are facing any issue or error with any of the tools inside PentestBox or the ones which are provided through [Toolsmanager](https://docs.pentestbox.com/toolsmanager.html), please submit yours [Bug Reports](https://docs.pentestbox.com/contributing.html/#submitting-bug-reports).

Is there any way I can give administrative rights to a particular tab?
----------------------------------------------------------------------------

By default PentestBox runs like a normal user, no administrative permission is required to launch it. But you might want to use some tool which requires administrative permission. In that case you need to right click on the tab and choose restart as admin, after that the tab will be given administrative rights.

How can I resize PentestBox?
------------------------------------

If you move your cursor along it edges, the cursor will change and you will be able to resize it by clicking and dragging, but this procedure is something not everyone is able to follow.

There is an alternative way to do this:

* Right click on the top bar and then click on settings.
* Then a new window will appear, uncheck “Hide caption Always” and save the settings as given below.
  ![](https://i.imgur.com/XClDvwz.png)
* Then PentestBox will look something like this.
  ![](https://i.imgur.com/z38sDac.png)
* You can now resize the window as you like. After that you can go to settings, check that option again and save settings. PentestBox will save your current windows size and will open as it is when you open it up next time.

Why is Metasploit not included in PentestBox?
------------------------------------------------

Metasploit contains exploits/payloads inside it, so when installed on Windows machines nearly all antiviruses and firewalls will put up warnings. Also, Metasploit officially instructs to disable antiviruses and firewalls while using it.

So in order to make PentestBox work without switching off any antiviruses programs, I have not included that. But if you are willing to switch off your antivirus program and want to use Metsaploit on Windows, you can download the "PentestBox with Metasploit" version from the [Download](https://pentestbox.com/#download) option.

Why is PentestBox throwing up red flags with it being malware?
--------------------------------------------------------------

* There are two Variants of PentestBox, one with Metasploit and one without Metasploit. Metasploit contains many exploits/payloads, so if you are using the version with Metasploit then your antivirus will definetly make warnings. But you don't need to worry about this, it won't infect your system, you can put the PentestBox folder in the exception list instead of switching off antivirus.
* But if you are using the PentestBox version without Metasploit, only some files can be detected as malicious depending on your antivirus. In case of Avira, below are some of the files detected malicious and the reason why it's detected:
    * C:/PentestBox/PentestBox.exe: If this is detected then you can use the PentestBox.bat file, even though the exe is just a compiled version of the PentestBox.bat file.
    * C:\PentestBox\bin\beef\modules\exploits\local_host\ie_ms12_004_midi\ie_ms12_004_midi.html: It's a part of the Beefproject, if deleted then some particular modules will not work.

Let me know if you have any concern regarding this issue.

Metasploit is not running. It's showing some kind of error.
--------------------------------------------------------------

First of all make sure that you have installed the ``PentestBox with Metasploit`` version in ``C:\PentestBox\`` and that any antivirus/firewall have been switched off right before installation (including Microsoft Windows Defender). Below are possible cases for Metasploit failure:
* If there is any ruby installation on your system, please remove it from the ``PATH``. In order to remove that, go to Control Panel > System > Advanced System Settings > Environment Variables. Then look for Ruby path in the ``PATH`` variable.
* In case if you are using the arabic language on your system, then you first need to type ``chcp 65001`` on the console in order to user Metasploit.
  ![](https://i.imgur.com/coUwpRG.jpg)

Why Ruby cannot be updated in PentestBox ?
--------------------------------------------------------

Most of the ruby based tools are not compatible with every version of Ruby, also ruby on windows has many issues. An update on ruby can make most of the tools non-functional. This is the main reason for not providing update functionality for Ruby.

