# mvno-web-theme
A WaveMaker web application base theme for mvno usecase

INSTRUCTIONS
============
Install Prerequisites
--------

* Node.js v10.17.x+

You can check if you have Node and npm installed by typing:
<pre>
$ node --version && npm --version
</pre>

If you need to upgrade or install Node, the easiest way is to use an installer for your platform. Download the .msi for Windows or .pkg for Mac from the [NodeJS website](https://nodejs.org/download/).

* Git
You can check if you have Git installed by typing:
<pre>
$ git --version
</pre>
If you don't have Git, grab the installers from the [git website](http://git-scm.com/).


Install Grunt & Bower
--------

Once you’ve got Node installed, install the Grunt and Bower:
<pre>
$ npm install --g bower grunt-cli
</pre>

(Make sure above commands execute with sudo/administrator permissions depending on OS eg, UNIX)

Setup WaveMaker Theme Repository
--------
To clone the mvno-web-theme repository, use git clone:

<pre>
 git clone https://github.com/wavemaker/mvno-web-theme.git
 cd mvno-web-theme
 npm install
</pre>

Understanding the Repository
--------
<pre>
+--src
|  +--web
|     +--style.less
|     +--variable.less
|     +--.wmproject.properties
|     +--theme.png
|     +--fonts/
+--dist
|  +--web.zip
+--Gruntfile.js
|
+--package.json
|
+--bower.json
</pre>

Fonts
-----
There will be references to Roboto regular fonts in the variables.less(src/web), to avail them please download Roboto regular fonts and paste them in fonts directory(src/web/fonts).

Build
--------
To build the WaveMaker Theme run the below command from mvno-web-theme directory

<pre>
cd mvno-web-theme
grunt themes
</pre>

Theme Zip
-----
There is a web.zip file which is complied theme source. This can be used to import the theme into your project with latest version. 
