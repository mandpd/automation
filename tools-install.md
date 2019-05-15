# CSU Development Working Group - Tools Installation

## Overview

To help leverage the whole team as we develop automation scripts, we’re proposing to use a common set of tools so that we can all assist in developing scripts and share the work product. We will be implementing a central repository that will provide access to the tools, implement a secure means of sharing, and allow us to customize the environment to support CSU’s specific needs.

In advance of the repository being established, you may want to obtain the primary tools we’ll be using now to gain some familiarity with them. These notes take you through obtaining and installing the tools one-by-one. Once the repository is established, we will make customized versions of the tools available, primarily as docker images. These will make the installation and maintenance of the tools easier than trying to work with the multiple versions and web sites involved with each tool (which is what you’re about to do!)

### Visual Studio Code

VS Code is a very popular code editor which is rapidly approaching the capability of full Integrated Development Environments like Visual Studio and Xcode. It is open source and benefits from a huge community of contributors. VS Code has extensions available to support a myriad of coding requirements, include Python, Ansible, Chef, Puppet, Javascript, ZAML, Typescript, markdown, and many, many, others. One key feature is Visual Share which allows multiple users to link their VS code instances together to allow team coding, execution, and debugging. This is a great environment if you’re new to scripting as it allows others to connect and review your code and provide remote edits and even run the same code in their local VS code.

### Node-RED

Node red is a visual programming tool originally designed to support IoT application development and execution. It provides a visual drag-and-drop capability to construct applications which will make the scripts that are developed by the group accessible and usable by non-scripters. The primary scripting language of node-RED is javascript, but we’ve extended it to also support Python scripts for custom logic. Nodes are the basic unit of programmability, and these are easily configured to perform specific tasks. Nodes can be linked together to form flows which can perform a complex series of tasks to accomplish a larger goal. For those more familiar with coding, it is possible to develop your own nodes that others can drag-and-drop into their flows.

### Github

Github is a web site that can be used to store and distribute scripts, programs, and many other document types. Scripts that you develop locally are managed using the git protocol which provides versioning of the code you write. Your scripts can be ‘pushed’ to github to provide a remote copy of the scripts to which you can give access to others. You can also ‘clone’ copies of scripts developed by others onto your local system without losing the versioning control. Access to public scripts on github is free, and you can set up an account now to see what’s available on github [here](https://github.com).

## Installation

### Python

Python is available from several sources. We’ll use the anaconda distribution which includes several other applications that will be useful. The download link is [here](https://www.anaconda.com/distribution/#download-section) We will be using the python 3 version which is on the left-hand side. Follow the default options and decline any of the optional downloads.

### Visual Studio Code

Visual Studio Code can be installed from [here](https://code.visualstudio.com/) Installers are available for Windows, Mac, and Linux. Just follow the default options. Once installed, there are a number of extensions that you should install. 

To do this, run visual studio. Select the last icon on the left hand side of the GUI (if you hover over icons you'll get a tooltip eventually - this one will say 'Extensions'). This will open the extensions viewer on the left hand side. Here you can enter a name or partial name of the extension you want to add, and you should see it listed below the search field. In many cases there will be multiple extensions matching your search phrase. To the right of each extension name you should see a 'cloud download' icon and the number of downloads for the extension next to it. (Widen the pane if this is not visible). A good guide for which extension to choose when there are multiple options is to pick the extension with the largest number of downloads as this is the most popular in its category. You can read more about an individual extension by clicking on it. To install the extension just click on the 'Install' button. Some extensions will require a reboot before they enable, but there will be a message to this effect when this occurs.

Feel free to explore and see the vast range of extensions available for VS Code. This is a big reason why it has become one of the most popular code editors (that, and the fact that it's free).

Please install the following extensions:


Extension | Comments
---------- | ---------------
Python | Once installed you may be asked to select the interpreter - there will be a drop down list and you should select the one with 'anaconda' in the filepath. (If you don't see this, there's something wrong with your python installation.)
GitLens | provides tight integration with Git and Github
Ansible | provides support for writing ansible scripts
Bash | If using a Mac or Unix OS
Colbalt2 Theme | My preferred theme - search for 'theme' to see others that are available
Live Share | This enables the live code sharing capability
Markdown PDF | This allows you to convert markdown documents to PDF (which is how this pdf was created)


### Git

We need a local implementation of git to provide versioning of our local files and to interact with the remote repositories on github. The download link is [here](https://git-scm.com/downloads) . Again, accept the defaults.

### Github Client

Github have their own client software that supports working with github through a gui rather than a command line. The download link is [here](https://desktop.github.com/). Accept the defaults.

### NodeJS

Node-RED is an application that runs on nodejs. The download link is [here](https://nodejs.org/en/). Select the LTS version and follow the defaults.

### Node-RED

Once nodejs is installed, follow the installation instructions [here](https://nodered.org/docs/getting-started/installation) (follow the text from the top of the page until 'Install via SNAP'). Once the installation completes, follow [these instructions](https://nodered.org/docs/getting-started/running) to run node-RED. Node-RED uses the browser as the main GUI, so once it is running open a browser and point it to [http://localhost:1880](http://localhost:1880) .

## Exploring the Tools

### Visual Studio Code

This [tutorial](https://code.visualstudio.com/docs/python/python-tutorial) describes writing an 'Hello World!' python script in Visual Studio Code. This is also a good test that everything is configured correctly.

### Node-RED

You can follow the instructions [here](https://nodered.org/docs/getting-started/first-flow) to create your first flow.
