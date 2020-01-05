# clientautomationusingAI

Automation of clients using ai technique.
The first attempt is, will be on an android client afterwards web client and finally iOS.
Since it is at its early stage things might go wrong and my be difficult to accomplish.
The main goal is to be able to get away from the traditional element location by rather using the appium classifier plugin
offered from  jlipps (see https://github.com/testdotai/appium-classifier-plugin)

What I have installed and used:

latest stable ubuntu verison  and a terminal
node(https://nodejs.org/en/)
npm
appium:(downloaded it from the source-http://appium.io/docs/en/contributing-to-appium/appium-from-source/index.html-) and read how appium is installed.

appium-doctor:(went to -https://github.com/appium/appium-doctor- to install appium tool) and cloned it and afterwards did (cd appium-doctor -> npm install --> npm run build --> node. ). Please check the following link: http://appium.io/docs/en/contributing-to-appium/appium-from-source/index.html

Install android-studio

Run from command line ./appium-doctor.js within appium-doctor folder you have cloned previously to see what is beeded or not that needs to be installed or fixed.


In my case under ~/.bashrc you need to have the following set: 

#Nodejs

VERSION=v12.14.0
DISTRO=linux-x64
export PATH=/usr/local/lib/nodejs/node-$VERSION-$DISTRO/bin:$PATH


#JAVA

export JAVA_HOME="/usr/lib/jvm/java-14-openjdk-amd64/bin"
export PATH=${JAVA_HOME}/bin:$PATH


#AndroidStudio

export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
export PATH=$PATH:$ANDROID_HOME/bundletool


#OpenCV

export OPENCV4NODEJS_AUTOBUILD_OPENCV_VERSION=4.1.0

Go to the README.md of https://github.com/testdotai/appium-classifier-plugin and try the rest
