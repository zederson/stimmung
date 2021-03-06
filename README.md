# Stimmung

Simple sentiment analysis for the German language

[![Gem Version](https://badge.fury.io/rb/stimmung.svg)](http://badge.fury.io/rb/stimmung) ![Installs](http://img.shields.io/gem/dt/stimmung.svg)


## Usage

```ruby

# use this to init with the default dictionaries
stimmung = Stimmung.new

# or this to init with your dictionaries
stimmung = Stimmung.new('my_dict1.txt', 'my_dict2.txt', '...')

# you can always load additional dictionaries later on with
stimmung.load_dictionary('my_dict.txt')

# and to get an analysis you just do
stimmung.score('irgendein toller text')
# => 0.5066 

# this score will be between -1 (super negative) and 1 (super positive)

```

## Dictionaries

The German dictionary is based on SentiWS.

SentiWS is licensed under a Creative Commons Attribution-Noncommercial-Share Alike 3.0 Unported License (http://creativecommons.org/licenses/by-nc-sa/3.0/).

The latest version of SentiWS can be found at http://wortschatz.informatik.uni-leipzig.de/download/

You can use the crude importer script to import new files in case there is a new version. Hey why don't you open an issue or make a pull request when that happens too? It would be appreciated :)

## Installation

    gem install stimmung
