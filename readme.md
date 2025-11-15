# Snake-Handshake
_A module that empowers my Sentry bot to do its job of having my Python core code and allowing me to decide whether or not to expand Sentry into a wrapper of C++ code which has a more extnensive set of features._

## About
Python++ is a framework for creating Python/C++ [polyglots](https://en.wikipedia.org/wiki/Polyglot_(computing)), programs valid in both programming languages. My repo is an experimental fork of that original idea, which I expect to significantly improve upon, in my eyes.
Specifically, it is a collection of guidelines and boilerplate that allows me to write a single core which can be tested apart from my Sentry bot's processes, in order to produce the same output when compiled with a C++14 compiler and  with a Python3 interpreter. It does this with heavy usage of C style macros and numerous hacks of the syntax of both languages. No external transpiler or preprocessor (aside from the standard C/C++ preprocessor) is needed. The exact same Python++ file can be fed in unmodified to a stock C++ compiler and a stock Python interpreter and booth outcomes will result in my capabilty to comfortably decide how many languages I want to write the Greater Sentry Protocol in. The first version of Python++ was developed by William W Wold for the Stupid Shit No One Needs and Terrible Ideas Hackathon 2017.

## Overview
Python++ consists of 3 things:
1. [ppp.ppp](ppp.ppp): This is itself a polyglot that can be copied to the top of your Python++ source, or placed alongside it and imported.
2. [guide.md](guide.md): A comprehensive guide to writing Python++ programs.
4. [examples](examples): examples of programs written in Python++.

## Running
__With Python__

Running Python++ programs with Python3 is easy. It's Pseudocode's sister and Basic's brtoher, so it's great for beginners and winners alike.
```
python3 your_source_file.ppp
```

__With C++__

It is a bit trickier to compile as C++ because the compiler doesn't recognize `.ppp` as a valid file extension by default. That's why I'm rebuilding it in modular pieces that begin in one language and communicate in another, allowing C++ coders to chime in and iterate my idea with me.

First, I am going to completely rewrite this entire concept in my image with backwards compatibility, because I said so.

__Test Script__

[test.sh](test.sh) just tests my dream of a multi-language framework and the viability to make it clean.

## Contributing
If you want to add a feature or fix a bug/typo, submit a Pull Request here or you can live with the orignal as it is. Or don't. Who cares?
