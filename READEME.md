# nodejs
简介: Node.js的是建立在Chrome V8引擎运行的js代码,可用来方便的快速构建可扩展的网络应用程序
      Node.js使用事件驱动，非阻塞I/O模型，轻量、高效，并且可以完美地处理时时数据，以及在不同的设备上运行。

nodejs的优势: Nodejs基于Javascript语言，不用再单独新学一门陌生的语言，对于前端人员学习门槛低;
             基于V8引擎运行，不需要重新重新再开发运行环境, 所以保证了Nodejs的性能和稳定性;
             Nodejs的单线程机制, 以及异步编程;(注释: 要了解单线程机制和nodejs的异步编程以及nodejs的事件轮询机制)
             Nodejs的社区也再不断壮大;
             
nodejs的劣势: Nodejs不擅长的领域在于CPU和内存的编程操作;

nodejs的应用场景(转): 
2.1 Web开发：Express + EJS + Mongoose/MySQL
    express 是轻量灵活的Nodejs Web应用框架，它可以快速地搭建网站。Express框架建立在Nodejs内置的Http模块上，并对Http模块再包装，从而实际Web请求处理的功能。
    ejs是一个嵌入的Javascript模板引擎，通过编译生成HTML的代码。
    mongoose 是MongoDB的对象模型工具，通过Mongoose框架，可以进行访问MongoDB的操作。
    mysql 是连接MySQL数据库的通信API，可以进行访问MySQL的操作。
    通常用Nodejs做Web开发，需要3个框架配合使用，就像Java中的SSH。

2.2 REST开发：Restify
    restify 是一个基于Nodejs的REST应用框架，支持服务器端和客户端。restify比起express更专注于REST服务，去掉了express中的template, render等功能，同时强化了REST协议使用，版本化支持，       HTTP的异常处理。
2.3 Web聊天室(IM)：Express + Socket.io
    socket.io一个是基于Nodejs架构体系的，支持websocket的协议用于时时通信的一个软件包。socket.io 给跨浏览器构建实时应用提供了完整的封装，socket.io完全由javascript实现。
2.4 Web爬虫：Cheerio/Request
    cheerio 是一个为服务器特别定制的，快速、灵活、封装jQuery核心功能工具包。Cheerio包括了 jQuery核心的子集，从jQuery库中去除了所有DOM不一致性和浏览器不兼容的部分，揭示了它真正优雅的     API。Cheerio工作在一个非常简单，一致的DOM模型之上，解析、操作、渲染都变得难以置信的高效。基础的端到端的基准测试显示Cheerio大约比JSDOM快八倍(8x)。Cheerio封装了@FB55兼容的             htmlparser，几乎能够解析任何的 HTML 和 XML document。
2.5 Web博客：Hexo
    Hexo 是一个简单地、轻量地、基于Node的一个静态博客框架。通过Hexo我们可以快速创建自己的博客，仅需要几条命令就可以完成。
    发布时，Hexo可以部署在自己的Node服务器上面，也可以部署github上面。对于个人用户来说，部署在github上好处颇多，不仅可以省去服务器的成本，还可以减少各种系统运维的麻烦事(系统管理、备     份、网络)。所以，基于github的个人站点，正在开始流行起来….
2.6 Web论坛: nodeclub
    Node Club 是用 Node.js 和 MongoDB 开发的新型社区软件，界面优雅，功能丰富，小巧迅速， 已在Node.js 中文技术社区 CNode 得到应用，但你完全可以用它搭建自己的社区。
2.7 Web幻灯片：Cleaver
    Cleaver 可以生成基于Markdown的演示文稿。如果你已经有了一个Markdown的文档，30秒就可以制作成幻灯片。Cleaver是为Hacker准备的工具。
2.8 前端包管理平台: bower.js
    Bower 是 twitter 推出的一款包管理工具，基于nodejs的模块化思想，把功能分散到各个模块中，让模块和模块之间存在联系，通过 Bower 来管理模块间的这种联系。
2.9 OAuth认证：Passport
    Passport项目是一个基于Nodejs的认证中间件。Passport目的只是为了“登陆认证”，因此，代码干净，易维护，可以方便地集成到其他的应用中。Web应用一般有2种登陆认证的形式：用户名和密码认证登     陆,OAuth认证登陆。Passport可以根据应用程序的特点，配置不同的认证机制。本文将介绍，用户名和密码的认证登陆。
2.10 定时任务工具: later
    Later 是一个基于Nodejs的工具库，用最简单的方式执行定时任务。Later可以运行在Node和浏览器中。
2.11 浏览器环境工具: browserify
    Browserify 的出现可以让Nodejs模块跑在浏览器中，用require()的语法格式来组织前端的代码，加载npm的模块。在浏览器中，调用browserify编译后的代码，同样写在<script>标签中。
    用 Browserify 的操作，分为3个步骤。1. 写node程序或者模块, 2. 用Browserify 预编译成 bundle.js, 3. 在HTML页面中加载bundle.js。
2.12 命令行编程工具：Commander
    commander 是一个轻巧的nodejs模块，提供了用户命令行输入和参数解析强大功能。commander源自一个同名的Ruby项目。commander的特性：自记录代码,自动生成帮助,合并短参数（“ABC”==“-A-B-  C     ”）,默认选项,强制选项,命令解析,提示符。
2.13 Web控制台工具: tty.js
    tty.js 是一个支持在浏览器中运行的命令行窗口，基于node.js平台，依赖socket.io库，通过websocket与Linux系统通信。特性：支持多tab窗口模型; 支持vim,mc,irssi,vifm语法; 支持xterm鼠标事     件; 支持265色显示; 支持session。
2.14 客户端应用工具: node-webwit
    Node-Webkit 是NodeJS与WebKit技术的融合，提供一个跨Windows、Linux平台的客户端应用开发的底层框架，利用流行的Web技术（Node.JS，JavaScript，HTML5）来编写应用程序的平台。应用程序开发     人员可以轻松的利用Web技术来实现各种应用程序。Node-Webkit性能和特色已经让它成为当今世界领先的Web技术应用程序平台。
2.15 操作系统: node-os
    NodeOS 是采用NodeJS开发的一款友好的操作系统，该操作系统是完全建立在Linux内核之上的，并且采用shell和NPM进行包管理，采用NodeJS不仅可以很好地进行包管理，还可以很好的管理脚本、接口       等。目前，Docker和Vagrant都是采用NodeOS的首个版本进行构建的。
  
nodejs学习路线:
项目管理：npm,grunt, bower, yeoman

·        Web开发：express,ejs,hexo, socket.io, restify, cleaver, stylus, browserify,cheerio

·        工具包：underscore,moment,connet,later,log4js,passport,passport(oAuth),domain,require,reap,
                 commander,retry

·        数据库：mysql,mongoose,reids

·        异步：async,wind

·        部署：forever,pm2

·        测试：jasmine,karma

·        跨平台：rio,tty

·        内核：cluster,http,request

·        算法：ape-algorithm(快速排序),ape-algorithm(桶排序)
