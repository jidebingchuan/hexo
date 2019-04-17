---
title: PHP 版本选择
date: 2013-08-21 13:57:07
tags: PHP
---

### PHP目前有三个主要版本：PHP4/PHP5/PHP6

PHP4由于太古老、对OO支持不力已基本被淘汰，不用考虑PHP4。

PHP6由于基本没有生产线上的应用，还基本只是一款概念产品，很多功能已在PHP5.3上实现，所以暂不考虑PHP6。

PHP5的版本目前还在维护的主要分三支：PHP5.3.x、PHP5.4.x和PHP5.5.x

PHP5.3之前的版本不值得考虑，因为某些功能缺陷或者BUG。

主流PHP程序对PHP5.3.x的兼容性最好，而每次版本号的升级带来的都是安全性和稳定性的改善，所以宜挑选最新的版本。目前PHP5.3系列最新的是PHP5.3.27。

2013-07-12 经过1个RC 上个版本是2013-06-07的5.3.26 修正了大约10个Bug以及几个安全漏洞。注意这将是5.3系列最后一个常规版本，PHP官方建议用户应该升级到 5.4或5.5 但安全更新会持续到明年。

而如果产品是自己开发自己使用，PHP5.4在某些方面更具优势，是部署项目值得考虑的版本。目前PHP5.4系列最新的是PHP5.4.18。



### 面向windows的php有以下几个版本

windows版本下载地址：http://windows.php.net/download/

Installer：可执行的MSI格式安装包。

Zip：解压即可用。和install版无区别。建议选择Zip版。

Debug Pack：带调试的php包。



### VC6与VC9是什么？

VC6就是legacy Visual Studio 6 compiler，就是使用这个编译器编译的。

VC9 就是 the Visual Studio 2008 compiler，就是用微软的VS编辑器编译的。

那我们如何选择下载哪个版本的PHP呢？

如果你是在windows下使用Apache+PHP的，请选择VC6版本。

如果你是在windows下使用IIS+PHP 的，请选择VC9版本。

提示：使用VC9版的时候需要有VC++2008的运行时环境(x86)。(x64)

提示：不要在apache下使用VC9的版本。

提示：php5.2官方只提供vc6的下载。

提示：php5.3官方提供了vc6和vc9的下载，但从php5.3.5之后只提供vc9版的下载。php5.3.5是最后一个带vc6版的。



### TS和NTS是什么？

TS 指 Thread Safe，即线程安全，一般在IIS以ISAPI方式加载的时候选择这个版本。

NTS 指 Non Thread Safe，即非线程安全，一般在IIS以FastCGI方式运行的时候选择这个版本，具有更好的性能。

提示：从PHP 5.3.0 开始发布的Windows版已经不支持ISAPI模式了，下载的php压缩包中没有php5isapi.dll，所以推荐FastCGI方式运行PHP。



### 如何查看当前运行的PHP的版本？

一个很简单的办法就是phpinfo();

Thread Safety disabled是NTS，enabled是TS

Configure Command看到VC98字样的是VC6，Compiler标明 MSVC9 (Visual C++ 2008) 的是VC9

