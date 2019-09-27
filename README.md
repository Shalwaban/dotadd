ADD - Ambisonics Decoder Description
========

### [dotadd-web-converter](https://smp-3d.github.io/dotadd-online-converter/) - [dotaddtool](https://github.com/smp-3d/dotadd.tools)


The .add-format stores data for Ambisonics decoding matrices. The purpose of the format is to merge all possible data types of already established formats and serve as an intermediate between software in case of compitability issues.

For this we offer two solutions: 
* a **library** for direct integration into developed software
* a **toolkit** for conversion between supported formats

Supporting these formats:
* [**IEM SimpleDecoder and AllRAD Decoder**](https://plugins.iem.at/)
* [**ambiX**](http://www.matthiaskronlachner.com/?p=2015)
* [**ICST ambidecode~**](https://www.zhdk.ch/forschung/icst/software-downloads-5379/downloads-ambisonics-externals-for-maxmsp-5381)
* [**ambdec**](http://kokkinizita.linuxaudio.org/linuxaudio/index.html)
* [**CSV**](https://en.wikipedia.org/wiki/Comma-separated_values)

Library
--------

To be useful in a variety of software solutions we offer libraries in different programming languages that can be used to read or write a .add-formatted file. These libraries differ in their design and thus have benefits or drawbacks. More specific information on the functionality and implementation can be found in the different repositories:

* [**C++**][rep_lib_cpp]
* [**JavaScript**][rep_lib_js]
* [**Python**][rep_lib_py]
* **Matlab** (coming soon)


**Toolkit**
--------

### [dotaddtool][rep_tool_console]

If running commands in an Unix-shell is the best way for you then use the **.add-console tool** which gives you the ability to read and write .add-files or convert between different formats for Ambisonics decoder matrices. 


### [.ADD-browser app][rep_tool_browser]

A convenient method to use the .add-format is the **.add-browser application**. Use drag-and-drop and a few clicks to configurate what you want and achieve a fast result with no need to install anything.

You can find it here: [coming soon]


### [.ADD-extractor VST][rep_tool_extractor]

Since non-dynamic decoders have a decoding matrix that is pre-calculated and acting passively it is possible to excite their inputs with an short impulse and then read the outcoming signal that has been processed. The .add-toolkit contains a *".add-exciter"* plugin being placed up-stream from a decoder of choice, and a *".add-reader"* being placed down-stream. 


Further information
--------

.ADD was developed by students of the [University of Applied Sciences Darmstadt](https://h-da.de/ "h_da - University of Applied Sciences Darmstadt")

Feel free to contribute!





[rep_all]: https://github.com/smp-3d	"dotadd Overview"

[rep_lib_py]:https://github.com/smp-3d/dotadd.py	".ADD Python - dotadd.py repository"
[rep_lib_js]:https://github.com/smp-3d/dotadd.js	".ADD JavaScript - dotadd.js repository"
[rep_lib_cpp]:https://github.com/smp-3d/libdotadd	".ADD C++ - libdotadd repository"
[rep_lib_m]:https://github.com/smp-3d/dotadd.m	"ADD MatLab - dotadd.m repository"

[rep_tool_console]:https://github.com/smp-3d/dotadd.tools	".ADD-console tool"
[rep_tool_browser]:https://github.com/smp-3d/dotadd-online-converter	".ADD-browser app"
[rep_tool_extractor]:https://github.com/smp-3d/dotadd-dec-ripper	".ADD-extractor VST"
