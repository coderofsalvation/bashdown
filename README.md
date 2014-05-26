bashdown
========

markdown to html converter with bash as templating language, written in 100% pure bash, macgyver-style documentation generator

### Usage ###

    cat bashdown/example.md | bashdown | markdown > example.html

That will turn [this](https://raw.github.com/coderofsalvation/bashdown/master/example/example.md) into :

<img src="https://raw.github.com/coderofsalvation/bashdown/master/example/example.png" style="border:1px solid #CCC"/>

### why ###

* to quickly write documentation
* portable
* unlimited possibilities
* markdown is nice, but has no template engine
* bash is a fullfledged template engine already
* everybody uses bash
* its installed everywhere

CREDITS: the amazingly portable markdown bashconverter was written by [Chad](https://github.com/chadbraunduin) 

### requirements ###

* BASH!
* bashfu ninjaskills (its worth the investment..really)

### Installation ###

    mkdir ~/bin 
    cd /tmp
    git clone https://github.com/coderofsalvation/bashdown.git
    git clone https://github.com/chadbraunduin/markdown.bash
    cp markdown.bash/markdown.sh ~/bin/markdown
    cp bashdown/bashdown ~/bin/.

### Example

In the 'example' directory you can see a simple wrapper which turns an markdown document into a nice styled html-document like so:
  
    ./mybashdown example.md > example.html

see the output [here](https://raw.githubusercontent.com/coderofsalvation/bashdown/master/example/example.html)

### Note ###

Put this in ~/.profile so you always have handson-access to your bashscripts in ~/bin:

     PATH="$HOME/bin:$PATH"

