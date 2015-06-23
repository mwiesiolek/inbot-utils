# Introduction

Inbot-utils is a collection of utility classes that we use at [Inbot](http://inbot.io). These are the kinds of utilities most engineers keep around and copy from project to project.

# Install from maven cental

[![Build Status](https://travis-ci.org/Inbot/inbot-datemath.svg)](https://travis-ci.org/Inbot/inbot-datemath)

```xml
<dependency>
  <groupId>io.inbot</groupId>
  <artifactId>inbot-utils</artifactId>
  <version>1.0</version>
</dependency>
```

# Overview

Look at the source code and unit tests for detailed overview. Most of the utilities are straightforward to use and don't require much in terms of dependencies.

Currently these classes are included:

- AESUtils: encrypt/decrypt blobs using AES with a randomized salt and specified key
- ArrayFoo: misc static methods for manipulating arrays and sets
- CompressionUtils: compress/decompess using gzip; convenient wrappers around the built in java compression classes
- HashUtils: misc utilities to create md5 sha1 and other hashes without having to deal with checked exceptions or arcane details on how to set this up
- Md5Appender: helper class to creat md5 hashes incrementally by appending objects to it.
- MiscUtils: equalsAny method that returns true if the first arg is equal to any of the remaining ones (varargs)
- StrategyEvaluator: varargs and Optional based implementation of the strategy pattern
- IOUtils: helper methods to quickly work with streams and readers in a responsible way
- Math: a few methods that are missing from java.lang.Math that are useful

This library requires Java 8.

# Bugs/fixes & license

This code is [licensed](https://github.com/Inbot/inbot-utils/blob/master/LICENSE) under the MIT license.

We welcome pullrequests but please respect that this is a small project and that we use it in production and can't change everything at will. That being said, we love your feedback, suggestions, and pull requests. All this means is that we want to keep things stable, simple, and backwards compatible unless there is a good reason otherwise.

Given the nature of this project and the license, we fully understand if people want to just grab some of the code and copy it over. The license allows this and we don't mind it if you do this at all. However, if doing, so, please retain a comment acknowledging our copyright and the license. Also, drop us a mention [@inbotapp](https://twitter.com/inbotapp).


# Changelog

 - 1.1 - Add a few more classes: Md5Appender, IOUtils, Math
 - 1.0 - Initial release
