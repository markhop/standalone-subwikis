# Standalone Sub-Wikis #

## Overview ##
[FitNesse](http://fitnesse.org) is a _"standalone [wiki](http://wiki.org/wiki.cgi?WhatIsWiki) and acceptance testing framework"_ that uses a page hierarchy similar to a filesystems directory structure.  This [Sub-Wiki](http://www.fitnesse.org/FitNesse.UserGuide.SubWiki) feature allows project pages to be isolated effectively providing namespace separation.

This project was created to investigate the possibility of creating standalone sub-wikis using the __fitnesse__ software to create the sub-wikis but keeping _FitNesse's_ own pages out of the source code repository.

## Implementation ##

The project provides..

- a _.gitignore_ file specifically tailored to keep all of _FitNesse's_ own pages out of the git repository
- _build.gradle_ a [Gradle](http://gradle.org) build file to start up the _FitNesse_ instance
- _gradle.properties_ used to specify the version of _FitNesse_ to use
- _plugins.properties_ the _FitNesse_ plugins files specifying how _FitNesse_ should behave
- _README.md_ this file...

## Dependencies ##

The project requires the following...

- Java (JRE/JDK) 1.6 minimum
- The [Gradle](http://gradle.org) build system
- a connection to the internet

## Usage ##

To use the project simply clone the github project and after ensuring the dependencies (above) are installed issue the following at the command line.

    gradle start

The first time this command is run FitNesse and all its dependencies will be downloaded prior to FitNesse being run up on port 8050.

    C:\Users\Mark\Documents\GitHub\standalone-subwikis>gradle start
    :copyToLib
    Download http://repo1.maven.org/maven2/org/fitnesse/fitnesse/20130530/fitnesse-20130530.pom
    Download http://repo1.maven.org/maven2/com/googlecode/java-diff-utils/diffutils/1.2.1/diffutils-1.2.1.pom
    Download http://repo1.maven.org/maven2/org/fitnesse/fitnesse/20130530/fitnesse-20130530-standalone.jar
    Download http://repo1.maven.org/maven2/com/googlecode/java-diff-utils/diffutils/1.2.1/diffutils-1.2.1.jar
    :start
    FitNesse (v20130530) Started...
    java -jar lib/fitnesse-standalone.jar -p 8050 is ready
    
    BUILD SUCCESSFUL
    
    Total time: 25.256 secs
    C:\Users\Mark\Documents\GitHub\standalone-subwikis>


To access the running FitNesse instance point your favourite browser at `http://localhost:8050`.  The instance is started in the background so the command shell can continue to be used for other tasks.  To shutdown the instance simply point your browser to `http://localhost:8050?shutdown`.



