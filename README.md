# Photon static site generator (experimental)

**Photon is a static site generator based on Neos CMS technology.**

## What is Photon?

* Content is stored in folders and files without needing a database
* A static version of the Neos Content Repository provides many of the same features like flexible and custom Node Types for structuring semantic content - by using folders and YAML files
* Content can be nested inside YAML files (but it  can always be split in separate files)
* Photon does not use a fixed one-to-one mapping between files for the content and its output, like many other SSGs
* Generating _something_ (it's not limited to HTML) from the content is fully flexible and based on Fusion (as one possible generator implementation)
* Fusion in Photon can use `FlowQuery` to traverse static nodes almost like in the original content repository
* For now it's an experiment to see how static site generation and Neos can be brought together

## Getting started

### Creating a new project

    composer create-project flowpack/photon-base-distribution -s dev photon-demo

### Generate content from the demo package

    ./flow generate:content Flowpack.Photon.Demo

See `Flowpack.Photon.Demo/Resources/Private/Fusion/Root.fusion` for a demo generator definition and `Flowpack.Photon.Demo/Resources/Private/Content` for the static content layout.

## Development

All development is done in https://github.com/Flowpack/photon-development-collection, expect to find a lot of loose ends and bugs.