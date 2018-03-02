
Denarius [DNR] NodeJS Statistics
=======================

[![Dependency Status](https://david-dm.org/carsenk/denariusstats/status.svg?style=flat)](https://david-dm.org/carsenk/denariusstats) [![Build Status](https://travis-ci.org/carsenk/denariusstats.svg?branch=master)](https://travis-ci.org/carsenk/denariusstats) [![Join the chat at https://gitter.im/denariusproject/Lobby](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/denariusproject/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link) [![Thinkful Pair on Node](https://tf-assets-staging.s3.amazonaws.com/badges/thinkful_repo_badge.svg)](http://start.thinkful.com/node/)

**Live Demo**: https://denarius.host

Denarius Node Statistics - NodeJS powered denariusd Stats.

View tons of Denarius related statistics including the current number of masternodes online in the Denarius network.

Table of Contents
-----------------

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Denarius Daemon Setup](#denarius-daemon-setup)
- [License](#license)

Features
--------

- View denariusd statistics
- View coinmarketcap statistics for DNR

-More features will be coming!

Prerequisites
-------------

- [denariusd](https://github.com/carsenk/denarius)
- [Node.js 6.0+](http://nodejs.org)
- Command Line Tools (Optional)
 - <img src="http://deluge-torrent.org/images/apple-logo.gif" height="17">&nbsp;**Mac OS X:** [Xcode](https://itunes.apple.com/us/app/xcode/id497799835?mt=12) (or **OS X 10.9+**: `xcode-select --install`)
 - <img src="http://dc942d419843af05523b-ff74ae13537a01be6cfec5927837dcfe.r14.cf1.rackcdn.com/wp-content/uploads/windows-8-50x50.jpg" height="17">&nbsp;**Windows:** [Visual Studio](https://www.visualstudio.com/products/visual-studio-community-vs)
 - <img src="https://lh5.googleusercontent.com/-2YS1ceHWyys/AAAAAAAAAAI/AAAAAAAAAAc/0LCb_tsTvmU/s46-c-k/photo.jpg" height="17">&nbsp;**Ubuntu** / <img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Logo_Linux_Mint.png" height="17">&nbsp;**Linux Mint:** `sudo apt-get install build-essential`
 - <img src="http://i1-news.softpedia-static.com/images/extra/LINUX/small/slw218news1.png" height="17">&nbsp;**Fedora**: `sudo dnf groupinstall "Development Tools"`
 - <img src="https://en.opensuse.org/images/b/be/Logo-geeko_head.png" height="17">&nbsp;**OpenSUSE:** `sudo zypper install --type pattern devel_basis`

Getting Started
---------------

The easiest way to get started is to clone the repository:

```bash
# Get the latest snapshot
git clone --depth=1 https://github.com/carsenk/denariusstats.git denariusstats

# Change directory
cd denariusstats

# Install NPM dependencies
npm install

# Or, if you prefer to use `yarn` instead of `npm`
yarn install

# Then simply start your app
node app.js

# Or, if you are using nodemon
nodemon app.js
```

**Note:** I highly recommend installing [Nodemon](https://github.com/remy/nodemon).
It watches for any changes in your  node.js app and automatically restarts the
server. Once installed, instead of `node app.js` use `nodemon app.js`. It will
save you a lot of time in the long run, because you won't need to manually
restart the server each time you make a small change in code. To install, run
`sudo npm install -g nodemon`.

Denarius Daemon Setup
------------------

You must have a Denarius daemon running on a local server or remote server (highly recommend using SSL)

Your configuration options should be set within your .env file, you can check the .env.example for examples

In your denarius.conf file (The Denariusd/QT configuration file) add the following to allow use of the stats.

```bash

server=1
rpcuser=yourusername
rpcpassword=yourpassword

```

License
-------

The MIT License (MIT)

Copyright (c) 2018 Carsen Klock

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
