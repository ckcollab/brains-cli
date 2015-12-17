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

##### `> brains push [dataset] [--name Name]`

requires `brains init` first. collects local source and pushes to server, optionally specifying
a dataset to run against.

Also allows a `--name` so you can mark specific pushes, like `--name "working layer activation function"`

##### `> brains results`

Opens up results in browser


`brains.yaml` examples
==================

Hello world
```yaml
run: python hello_world.py
content: hello_world.py
```

Hello world with glob file pattern
```yaml
run: python hello_world.py
content: *.py
```

Hello world multiple individual files
```yaml
run: python hello_world.py
content:
 - hello_world.py
 - test_hello_world.py
 - yo_momma.dataset
```
