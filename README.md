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




