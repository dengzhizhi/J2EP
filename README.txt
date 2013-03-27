Thanks for wanting to try the jEasy Extensible Proxy!
You can always find the latest version of this program at
http://sourceforge.net/projects/j2ep/


jEasy Extensible Proxy (J2EP) is a reverse proxy running on
a J2EE engine. J2EP is licensed under the Apache License,
Version 2.0. More information about the license can be found
in the file LICENSE or at 
http://www.apache.org/licenses/LICENSE-2.0


This is the source distribution of J2EP, if you only want to
run the proxy download the normal release instead.

The following files and directories are included in this 
release:

	* /src – The source
	* /docs – The documentation
	* /docs/api – Javadoc
	* /docs/release-notes.html – Notes specific to this release
	* README(.txt) – This file, containing basic information
	  concerning all releases
	* LICENSE – The apache 2.0 license
	* build.xml - Ant build script to compile the source
	* build.properties.default - Basic properties for build


To compile J2EP you will need an environment with the J2EE 
specific APIs running and JDK 1.4.2 or greater. But there are
also some third party libraries needed for the compile. These
aren't included in this release but can be downloaded from 
their respective webpages. The following libraries are needed.

	* commons-httpclient – http://jakarta.apache.org/commons/httpclient/
	* commons-digester - http://jakarta.apache.org/commons/digester/
	* commons-codec - http://jakarta.apache.org/commons/codec/
	* commons-beanutils - http://jakarta.apache.org/commons/beanutils/
	* commons-logging - http://jakarta.apache.org/commons/logging/
	* junit - http://www.junit.org
	* cactus - http://jakarta.apache.org/cactus/

Some additional libraries are needed as well in order to get
cactus running, such as aspectjrt, these are however included
with cactus.

When you have set up your environment for the build the easiest
way to compile the classes is to use ant to run the included
build.xml. Before you can run the build file you will have to
supply a build.properties first. This file isn't included in 
the relase since it contains sensitive information (including
username and password for tomcat). More information on which 
parameters are needed for the build are given in build.xml. 

Before running the compile or release task (release will create
a WAR) you can run the download task. This will download all
the needed libraries to make for an easy compile. There is one
thing to note about this, you will need the junit.jar in your
ANT_HOME/lib.