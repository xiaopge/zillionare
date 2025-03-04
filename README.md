![](http://images.jieyu.ai/images/hot/zillionbanner.jpg)

<h1 align="center">大富翁AI量化社区欢迎您!</h1>

<p align="right">
<a href="https://zillionare.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/zillionare/badge/?version=latest"></img></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
</p>




大富翁是一个模块化、微服务架构的开源AI量化框架，提供行情数据的本地化存储，高速分布式行情服务，回测框架，策略因子，也提供机器学习和深度学习策略模型。

**NOTE**

本项目用于统领Zillionare各子项目，主要目的是提供一般性文档和公共信息。比如，Zillionare子项目遵循同样的开发规范，这份开发规范的详细说明就在本项目中提供。具体部署、使用各子项目，请见各子项目文档。

除非是协助撰写文档，请不要clone本项目库，也不要通过 ``pip install zillionare`` 来安装本项目。您应该根据自己的需求，安装zillionarer的子项目。

大富翁由一系列子项目组成：

## Omicron

[Omicron](https://github.com/zillionare/omicron>) 提供了数据的本地存储读写和其它基础功能，比如交易日历和时间，Triggers，类型定义等。它是zillionare各子项目依赖的数据访问sdk。在您安装了Omega服务器之后，就通过Omicron这个sdk来使用行情数据。

[使用文档](https://zillionare-omicron.readthedocs.io/zh_CN/latest/>) [项目地址](https://github.com/zillionare/omicron)

## Omega

[Omega](https://github.com/zillionare/omega>) 是基于Sanic构建的微服务，它通过行情适配器来收发数据，通过Omicron来将这些数据存储到本地。Omega也是行情同步任务的管理者。

通过前置Nginx，就可以分布式方式提供行情数据服务。

[使用文档](https://zillionare-omega.readthedocs.io/zh_CN/latest) [项目地址](https://github.com/zillionare/omega)

## Alpha 

策略服务器。运行定义的各种策略，并发出交易信号。

## Epsilon 

Web控制台

## Gamma

交易网关。接收Alpha发出的交易信号，执行交易。这部分也可以集成在Alpha中。

## jqadaptor

JoinQuant行情数据适配器。

# 项目状态

截止2020年11月，大富翁已通过Omega提供高速分布式行情服务。部署Omega之后，即可通过Omicron（行情数据访问SDK）来请求行情数据和市值数据。


| 项目名称  | 最新版本 | 状态  | 说明                 |
|-----------|----------|-------|--------------------|
| Omega     | 0.6      | alpha | 高速分布式行情服务器 |
| Omicron   | 0.6      | alpha | 行情数据SDK          |
| jqadaptor | 0.2.x    | alpha | Joinquant行情适配器  |


## 更多

进一步了解大富翁，请跳转到 [文档](https://zillionare.readthedocs.io/en/latest/) 进一步阅读，谢谢！

## 加入社区

 * QQ群: 142961883
 * 头条号: 解语科技
 * 知乎圈子： Python与量化交易

<p align="center">
<img src="http://images.jieyu.ai/images/hot/qq.png" height="72px">
<img src="http://images.jieyu.ai/images/hot/logo-128-transparent.png" height="72px">
<img src="http://images.jieyu.ai/images/hot/quant-logo.jpg" height="72px">
</p>


