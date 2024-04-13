# Programming 2 - Exercise 0 : Setting-up VSCode and Scala

This page provides a step-by-step guide to install Scala 3 and/or Visual Studio Code (VSCode) on your computer, as well a some useful plugins. If you are using the lab computers at the University of Regensburg (CIP-Pools), you can directly start VSCode and jump to the part about Scala extensions.

*Warning:* It's essential to ensure that the paths to your projects do not contain spaces, special characters, or non-English letters. This is especially relevant on Windows, where historically, issues arose with usernames containing spaces or special characters.

## Tool installation

### VSCode Installation

* Open your favourite web browser and go to this webpage: https://code.visualstudio.com/download
* Download the executable corresponding to your OS and follow the instructions.

### Scala Installation

We recommend that you use VSCode to do the course exercises. In this case, it is not necessary to install Scala separately, the VSCode Scala extensions (below) suffice. If you prefer, however, you can also install Scala and the Scala build tool `sbt` yourself and use any other IDE or text editor.

* Open your favourite web browser and go to this webpage: https://docs.scala-lang.org/getting-started/index.html
* Follow the instruction related to your OS
* You may need to restart your terminal, log out, or reboot in order for the changes to take effect


### Scala Extension for VSCode

The extension "Scala (Metals)" adds various kinds of functionality to work with Scala to VSCode. To install this extension:

* Change to the "Extensions" pane and search for "Metals"
* In command line: https://marketplace.visualstudio.com/items?itemName=scalameta.metals

## Scala Hello World: Your First Project in Scala

### From this github repository

This repository contains a simple hello-world project that you can use to get started.

* You first need to create a local copy of the repository contents on your computer. If you have `git` installed on your computer, you can *clone* the repository using the command `git clone https://github.com/ur-tcs/programming-2-ex-0.git`, which will copy over all files to a sub-directory of your current directory. Alternatively, in your web browser you can download the repository contents by clicking on the green `<code>` button, selecting `Download ZIP`, and then unpacking the downloaded zip file.
* Change to the directory `programming-2-ex-0`: `cd programming-2-ex-0/hello-world`.
* Eventually VSCode will ask you to import the build, please click “Import build”
* Run `sbt`
* Type `run`

### By Yourself
* Create a folder `programming-2-ex-0`
* Go into this folder: `cd programming-2-ex-0`
* Run `sbt new scala/scala3.g8`
* Give a name to your project (for example, `hello-world`)
* Go into your project: `cd hello-world`
* Eventually VSCode will ask you to import the build, please click “Import build”
* Run `sbt`
* Type `run`

⚠️ You need to be in the folder `programming-2-ex-0/hello-world` to be able to use `sbt`!

Congrats, you have successfully compiled your first program in Scala! Feel free to explore the project to get familiar with the syntax and the file hierarchy. 


## What Are Those Files?
Here is the initial project that you have downloaded: 
```
- hello-world
    - project (sbt uses this for its own files)
        - build.properties
    - build.sbt (sbt's build definition file)
    - src
        - main
            - scala (all of your Scala code goes here)
                - Main.scala (Entry point of program) <-- this is all we need for now
```

When you compiled it, new files appears. Do not pay too much attention to them for now, you are going to work with `Main.scala`, at least at the beginning. 

## Exercises Management for this Course
* Each exercise if going to be on a different github repository. We advice you to create a folder (for example, `ProgrammingII`) and to put all exercises within, in order to have the following hierarchy: 
```
- ProgrammingII
    - programming-2-ex-0
    - programming-2-ex-1
    - ...
```
* When we ask you to type and/or run a specific command (for instance, `git clone myProject`), we can directly give you the command or write it that way: ```$ git clone myProject`. The `$` symbol is called the prompt and isn’t part of the command. It’s a convention used to indicate that the following command should be executed in a terminal.
