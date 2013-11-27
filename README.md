bashdown
========

markdown to html converter with bash as templating language, written in 100% pure bash, macgyver-style documentation generator

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

### Usage ###

    cat bashdown/example.md | markdown | bashdown > example.html

That will turn [this](https://github.com/coderofsalvation/bashdown/blob/master/example.md) into [this](https://github.com/coderofsalvation/bashdown/blob/master/example.html).

### Note ###

Put this in ~/.profile so you always have handson-access to your bashscripts in ~/bin:

     PATH="$HOME/bin:$PATH"

