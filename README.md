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

```brains push [dataset]``` 
requires `brains init` first. collects local source and pushes to server, optionally specifying
a dataset to run against.

```brains results```
Opens up results in browser

TODO:

 - [ ] init command to make `brains.yaml`
 - [ ] send file to server
 - [ ] view results in browser
