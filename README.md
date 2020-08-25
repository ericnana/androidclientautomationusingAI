# clientautomationusingAI

Automation of clients using ai technique.
The first attempt is, will be on an android client afterwards web client and finally iOS.
Since it is at its early stage things might go wrong and my be difficult to accomplish.
The main goal is to be able to get away from the traditional element location by rather using the appium classifier plugin
offered from  jlipps (see https://github.com/testdotai/appium-classifier-plugin)

What I have installed and used for android client automation: Please avoid using sudo even though it is really temptative especially when trying to install appium
1) latest stable ubuntu version  and a terminal
2) node(https://nodejs.org/en/) and npm
3) appium:(downloaded it from the source-http://appium.io/docs/en/contributing-to-appium/appium-from-source/index.html-) and read how appium is installed.
4) appium-doctor:(went to -https://github.com/appium/appium-doctor- to install appium tool) and cloned it and afterwards did (cd appium-doctor -> npm install --> npm run build --> node. ). Please check the following link: http://appium.io/docs/en/contributing-to-appium/appium-from-source/index.html

5) Install android-studio

6) Run from command line ./appium-doctor.js within appium-doctor folder you have cloned previously to see what is beeded or not that needs to be installed or fixed.


7) Go to  ~/.bashrc you need to have the following set: 

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

8) Install selenium and start it as well https://www.npmjs.com/package/selenium-standalone
9) Go to the README.md of https://github.com/testdotai/appium-classifier-plugin and try the rest
10) Start appium (node . -a localhost -p 4723). 4723 is the default port.
11) To run the test go to the folder where the test is located in the terminal and do: mocha --timeout 30000 mytest.js. (You might have to install mocha by doing the following :npm install -g mocha)
