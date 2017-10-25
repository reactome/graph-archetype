[<img src=https://user-images.githubusercontent.com/6883670/31999264-976dfb86-b98a-11e7-9432-0316345a72ea.png height=75 />](https://reactome.org)

Reactome Graph Core - Quickstart Maven Archetype
===============================================

## Introduction
The project is a Maven archetype for Reactome Graph Core.

## Prerequisites

- JDK 8
- Maven 3

### Create a project

```console
    mvn archetype:generate \
        -DarchetypeGroupId=org.reactome.maven.archetypes \
        -DarchetypeArtifactId=graph-archetype \
        -DarchetypeVersion=1.0.0 \
        -DgroupId=your.groupid \
        -DartifactId=your-artifactId \
        -Dversion=0.0.1-SNAPSHOT \
        -DarchetypeRepository=http://www.ebi.ac.uk/Tools/maven/repos/content/repositories/pst-release
```

:memo: The above command will bootstrap a project using the archetype published here: http://www.ebi.ac.uk/Tools/maven/repos/content/repositories/pst-release

### Create a new project in IntelliJ

* Create new project `File > New > Project`
* Click Maven on the left hand side of the new project dialog
* Check `Create from archetype`
* Click the `Add Archetype` button
* Set `Group Id` to `org.reactome.maven.archetypes`
* Set `Artifact Id` to `graph-archetype`
* Set `Version` to `1.0.0`
* Set `Repository` to `http://www.ebi.ac.uk/Tools/maven/repos/content/repositories/pst-release`
* Click next and create the project

:memo: If you would like to create a project using archetype published in your local repository, skip repository field and make sure it is installed locally (see below).

### Install archetype locally

To install the archetype in your local repository execute the following commands:

```console
    git clone https://github.com/reactome/graph-archetype.git
    cd graph-archetype
    mvn clean install
```

### Create a project from a local repository

Create a new empty directory for your project and navigate into it and then run:

```console
    mvn archetype:generate \
        -DarchetypeGroupId=org.reactome.maven.archetypes \
        -DarchetypeArtifactId=graph-archetype \
        -DarchetypeVersion=1.0.0 \
        -DgroupId=your.groupid \
        -DartifactId=your-artifactId \
        -Dversion=0.0.1-SNAPSHOT
```

:memo: The above command will bootstrap a project using the archetype published in your local repository.
