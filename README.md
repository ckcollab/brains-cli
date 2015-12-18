brains-cli
==========

Command line interface to the brains project.


installation
============

```pip install brains```



usage
=====

##### `> brains init`

asks for user information and how to run the program, saves to `brains.yaml` in current directory

##### `> brains push [--dataset iris] [--description "My first try"] [--dont-wait-up]`

requires `brains init` first. collects local source and pushes to server. `--dont-wait` will make the call return immediately and not wait for results

##### `> brains results`

TODO: Opens up results in browser


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

Hello world multiple individual files AND glob patterns
```
run: python hello_world.py
content:
 - hello_world.py
 - test_hello_world.py
 - yo_momma.dataset
 - src/*.py
```
