
''' http://nodered.org/docs/getting-started/installation.html '''

Install node.js

Node-RED supports node.js 0.10.x and later. We recommend the use of node.js LTS.

Note: Node.js 7.x is under active development and is not recommended for a stable base. Many 3rd party node packages may not yet fully support Node 6.x and later, especially if they contain a binary component. Check with the author of the package if you are not sure.
You can get the latest Long Term Support (LTS) version of Node 4.x from:


  Linux Binaries: 32-bit or 64-bit
  Max OS X Installer: Universal
  Windows Installer: 32-bit or 64-bit

It is often easiest to use a packaged version specifically for your operating system.

We also have specific instructions available for certain hardware platforms:

Raspberry Pi
BeagleBone Black
Other download options are available here.

Install Node-RED

The easiest way to install Node-RED is to use node’s package manager, npm. Installing it as a global module adds the command node-red to your system path:

   sudo npm install -g --unsafe-perm node-red
   
Note: you should not use npm 1.x to install Node-RED. You can upgrade to the latest npm 2.x version with the command: sudo npm install -g npm@2.x

Note: sudo is required if running as a non-root user on Linux/OS X. If running on Windows, you will need to run in a command shell as Administrator, without the sudo command.

Note: During the install some errors may be reported by the node-gyp command. These are typically non-fatal errors and are related to optional dependencies that require a compiler in order to build them. Node-RED will work without these optional dependencies, but you may find additional node modules that require the ability to compile native code. You can find out how to install the node-gyp compiler dependencies here.

Next

Once installed, you are ready to run Node-RED.

Alternative install methods

Download a release

You can download the latest release from here. The zip contains a top-level folder called node-red-X.Y.Z where X.Y.Z is the version number. Once extracted, from within that top-level folder, run the following command:

  npm install --production
  
For Development - from GitHub

Running the code from GitHub is only intended for users who are happy to be using development code, or for developers wanting to contribute to the code.

You can clone the source repository directly from GitHub:

  git clone https://github.com/node-red/node-red.git
  
Once cloned, the core pre-requisite modules must be installed :

  cd node-red
  npm install
  
Note: when running from a clone of the git repository, it is necessary to install all dependencies, not just the production level ones. This is why the --production option should not be used.
You will also need to install grunt-cli in order to build the application before you can use it. This must be done globally.

  sudo npm install -g grunt-cli
You can then build and run the application

grunt build
node red
Next steps

Once installed, you are ready to run Node-RED.
