# useful-for-development

# Introduction
A collection of useful, opinionated guides to help with development.

## Table of Contents Ubuntu

1. **[Installing Java Versions](#1-installing-java-versions)**
2. **[Switching Java Versions](#2-switching-java-versions)**

---

### 1. Installing Java Versions
This guide shows you how to install Java without *apt*.
In the following example i'm installing Java 16 from AdoptOpenJDK.
<br>
1. Get a build you like:
#### OpenJDK Builds:
* [AdoptOpenJDK](https://adoptopenjdk.net/)
* [Amazon Corretto](https://aws.amazon.com/de/corretto/)
* [Microsoft Build of OpenJDK](https://docs.microsoft.com/de-de/java/openjdk/download)

There are of course many more... Just choose one you like.
  
2. Extract the downloaded file. In my case it is a *tar.gz*.

`tar -xf OpenJDK16U-jdk_x64_linux_hotspot_16.0.1_9.tar.gz`
   

3. Move the extracted folder to */usr/lib/jvm*

`sudo mv jdk-16.0.1+9/ /usr/lib/jvm/`


4. Use *update-alternatives* to install

`sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-16.0.1+9/bin/java 1`

That is all. Have fun :coffee:
---

### 2. Switching Java Versions
With *update-alternatives* it is a easy as:
<br>
`sudo update-alternatives --config java`
<br>
and choose an installed version.

---
