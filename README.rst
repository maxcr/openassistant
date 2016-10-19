OpenAssistant
=============

Maintained by the `OpenAssistant <http://www.openassistant.org/>`__ 




Installation
------------

* `Arch Linux <https://www.archlinux.org/>`_ or `Ubuntu Linux <http://openassistant.org/forum/support/ubuntu-16-04-installation/>`_ (Testing Soon on `macOS <https://www.apple.com/macos>`_)

`mkdir -p ~/src && git clone https://github.com/maxcr/openassistant ~/src/`

`yaourt pocketsphinx`

`sudo pacman -S festival festival-english festival-us`

echo "(Parameter.set 'Audio_Required_Format 'aiff)
(Parameter.set 'Audio_Method 'Audio_Command)
(Parameter.set 'Audio_Command \"paplay $FILE --client-name=Festival --stream-name=Speech\")" > ~/.festivalrc

`cd ~/src && bash ./assistant.sh`

Useful Tools
------------

* aplay - console audio player
* pamixer - portaudio volume control
* plaympeg - console mp3 player
* projectm - visualizations responsive to sound
* wmctrl - window manager control. opening, closing, resize, switch windows. 
* xdotool - command line x automation tool
* xvkbd - virtual keyboard for x

Running OpenAssistant
---------------------

* Install dependencies and tools.

* Download and unpack the latest ``openassistant-master.zip`` package.

* Edit ``assist.sh`` to configure desired variables, then save.

* Make ``assist.sh`` executable with: ``$chmod +x ./assist.sh``

* Run ``./assist.sh``. Global variables will be set and ``assistant.py`` will launch.

* If ``./etc/commands.json`` has changed and your machine is online, a new dictionary and language model will be created via the `Sphinx Knowledge Base Tool <http://www.speech.cs.cmu.edu/tools/lmtool.html>`__.

* Say "Hello!" :) To mute, say "Be quiet" or "Silence". To unmute, say "Talk to me". 

* To quit, say "Goodbye" or "Farewell."

* To change assistant commands and language, edit ``./etc/commands.json``. Exit and relaunch ``assist.sh``.

* For help, you can receive support in the `OpenAssistant Forum <http://openassistant.org/community/>`_.


Next Steps
----------

* Port OpenAssistant to multiple Linux distributions, beginning with Ubuntu

* Enable dynamic voice and instant name changes via spoken commands

* Configure syntax and actions via spoken commands

* Install internal language model translation

* Improve speech recognition and synthesis

* Long-term memory & machine learning

* Web scraping & information analysis

* Establish multiple default 'personalities' and plug-in functions

* Port OpenAssistant to all operating systems and devices

* Galactic Exploration!


Join Us!
--------

Join our development working group at: http://www.openassistant.org
