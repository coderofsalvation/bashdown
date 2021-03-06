bashdown
========

markdown to html converter with bash as templating language, written in 100% pure bash, macgyver-style documentation generator

### Usage

    $ cat foo.md | bashdown
    (produces markdown with evaluated values)

    $ cat foo.md | bashdown --html
    (evaluates template and produces html)

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

### Custom Markdown Chain

The '--html' makes usage of github's markdown processor, but you can use your own.
In the 'example' directory you can see a simple wrapper which turns an markdown document into a nice styled html-document like so:
  
    ./mybashdown example.md > example.html

see the output [here](https://raw.githubusercontent.com/coderofsalvation/bashdown/master/example/example.html)

### Note ###

Put this in ~/.profile so you always have handson-access to your bashscripts in ~/bin:

     PATH="$HOME/bin:$PATH"

