---
title: How to setup a blog with Hexo and Github
date: 2017-04-30 22:18:40
tags: [Hexo, Github, Blog]
categories: Hexo
---
Start your blog with [Hexo](https://hexo.io/) and [Github](https://github.com/) in 5 minutes.

<!-- more -->

## Prerequisites

+ [Git](https://git-scm.com/)
+ [Node.js](https://nodejs.org/en/)

### Install Git
Follow [Git](https://git-scm.com/)

### Install Node.js
The best way to install Node.js is with [nvm](https://github.com/creationix/nvm).

Install NVM:
``` bash
$ curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | sh
```

Install Node.js with NPM:
``` bash
$ nvm install stable
```

After the installation, you can test **node** and **npm** by running the commands:
``` bash
$ node -v
v7.9.0
$ npm -v
4.2.0
```

## Install Hexo
Once all the requirements are installed, you can install Hexo with npm.
``` bash
$ npm install hexo-cli -g
```

To test the installation
``` bash
$ hexo -v
hexo: 3.3.5
hexo-cli: 1.0.2
os: Darwin 16.5.0 darwin x64
http_parser: 2.7.0
node: 7.9.0
v8: 5.5.372.43
uv: 1.11.0
zlib: 1.2.11
ares: 1.10.1-DEV
modules: 51
openssl: 1.0.2k
icu: 58.2
unicode: 9.0
cldr: 30.0.3
tz: 2016j
```

**NOTE:** If you see ERRORs like below (e.g. on Mac OS)

> { Error: Cannot find module ‘./build/Release/DTraceProviderBindings' … code: 'MODULE_NOT_FOUND' }
> { Error: Cannot find module './build/default/DTraceProviderBindings' … code: 'MODULE_NOT_FOUND' }
> { Error: Cannot find module './build/Debug/DTraceProviderBindings' …’MODULE_NOT_FOUND’ }

reinstall the hexo-cli with **\-\-no-optional**
``` bash
$ sudo npm uninstall hexo-cli -g
$ sudo npm install hexo-cli --no-optional -g
```


## Setup Blog
Once Hexo is installed, run the following commands to build your Hexo blog.

Init your blog
``` bash
$ hexo init <anyfolder>
$ cd <anyfolder>/
$ npm install
```

Edit **_config.yml** as desired
``` yml
# Site
title: MrSeal
subtitle:
description: MrSeal's Blog
author: Fei Chen
language: en
timezone: Europe/Dublin

# URL
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: http://mrseal.github.io
root: /
permalink: :year/:month/:day/:title/
permalink_defaults:
```

Run and test the Hexo server on your local
``` bash
$ hexo server
INFO  Start processing
INFO  Hexo is running at http://localhost:4000/. Press Ctrl+C to stop.
```
Now, you should be able to see your blog at http://localhost:4000/.

**NOTE:** If you see ERRORs like below (e.g. on Mac OS)

> { Error: Cannot find module ‘./build/Release/DTraceProviderBindings' … code: 'MODULE_NOT_FOUND' }
> { Error: Cannot find module './build/default/DTraceProviderBindings' … code: 'MODULE_NOT_FOUND' }
> { Error: Cannot find module './build/Debug/DTraceProviderBindings' …’MODULE_NOT_FOUND’ }

run this
``` bash 
$ npm install hexo --no-optional
```

## Deploy Blog to Github
Now you can deploy your the blog to your github, and make it online to public.

First of all, you have to head over to [github](https://github.com/) and create a new repository named **username.github.io**, where *username* is your github username.

Then edit settings in **_config.yml**
``` yml
# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: https://github.com/username/username.github.io.git
  branch: master
```

Install [hexo-deployer-git](https://github.com/hexojs/hexo-deployer-git).
``` bash
$ npm install hexo-deployer-git --save
```

Deploy the blog
``` bash
$ hexo deploy
```

At this point, you should be able to see your blog at http://username.github.io.


## Write a New Post

``` bash
$ hexo new {postname}
$ vi source/_posts/{postname}.md
# generate static files and deploy
$ hexo generate -d
```


## Further Reading
* Hexo: https://hexo.io/
* Hexo Themes: https://hexo.io/docs/themes.html
* Theme Samples: https://hexo.io/themes/
* Github Markdown: https://guides.github.com/features/mastering-markdown/

