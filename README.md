brains-cli
==========

Command line interface to the brains project.


installation
============

```pip install brains```



usage
=====

```brains init```

asks for user information and how to run the program, saves to `brains.yaml` in current directory

```brains push [dataset] [--name Name]``` 

requires `brains init` first. collects local source and pushes to server, optionally specifying
a dataset to run against.

Also allows a `--name` so you can mark specific pushes, like `--name "working layer activation function"`

```brains results```

Opens up results in browser

TODO:

 - [ ] init command to make `brains.yaml`
 - [ ] send file to server
 - [ ] view results in browser
 - [ ] handle single/glob file pattern (`import glob; glob.glob("README.md")` still works no need to differentiate between single file and glob)
 - [ ] handle ARRAY file pattern
 - [ ] upload to pypi


`brains.yaml` examples
==================

Hello world
```
run: python hello_world.py
content: hello_world.py
```

Hello world with glob file pattern
```
run: python hello_world.py
content: *.py
```

Hello world multiple individual files
```
run: python hello_world.py
content:
 - hello_world.py
 - test_hello_world.py
 - yo_momma.dataset
```
