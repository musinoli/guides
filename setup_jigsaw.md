# How to setup JDK 9 / Jigsaw on MacOSX

1. download the latest jdk from https://jdk9.java.net/jigsaw/ and run the following in the download directory:

    `tar -xvf jigsaw-jdk-9*.tar --directory /Library/Java/JavaVirtualMachines/`

    this will extract the contents of the tar archive into the appropriate location for JDKs on your machine

2. ensure your bash profile file (_~/.bash_profile_) includes the following export of java home:

    `export JAVA_HOME=$(/usr/libexec/java_home)`

3. run the following to incorporate the above

    `source ~/.bash_profile`

    and that's it! 
    ___
    running `java -version` should now return something similar to the below:
    `java version "9-ea"`

    nice reference:
    https://www.mkyong.com/java/how-to-set-java_home-environment-variable-on-mac-os-x/

