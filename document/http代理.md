# http代理
http代理，对于大部分程序员来说应该都是用过的，而作为前端，我一般用它来进行跨域访问。当然http代理的功能有很多，比如拦截，监控，过滤，缓存等这些都可以通过http代理来实现。
### 什么是http代理？
http代理，对于客户端和服务器来说就是一个中间人的角色，对于连接它的客户端来说，它是服务器，对于它连接的服务器来说，它是客户端，而http代理主要就是来回传送客户端和服务器之间的http报文。
### http代理有什么功能？
http代理可以实现的功能比较多，比如：拦截，监控，过滤，web缓存，跨域，反向代理等。这些功能都可以通过代理来实现。

1、拦截功能：

比如我们需要拦截用户登录，如果用户已经登录，那么就直接返回页面，如果用户还没有登录，就重定向到用户登录页面，引导用户登录。或者页面存在权限控制，针对不同权限返回不同页面信息。

2、监控功能：

比如我们需要监控代码异常情况进行上报，那么我们需要监控特定的请求接口，如果有请求，我们就将异常进行上报。

3、过滤功能：

比如我们可以设置有些人可以访问我们的网站，有些人不能访问我们的网站。

4、web缓存功能：

每次请求一个页面时，代理服务器都会检查这个页面是否已经缓存在本地，如果在，就直接返回页面，如果不在，那么再向目标服务器发送请求获取页面，并缓存在代理服务器本地。

5、跨域功能：

我们经常需要跨域访问一些服务器上的数据，这个时候我们可以在同域下创建一个代理服务器，然后由代理服务器去请求不同域名下的服务器上的数据。

6、反向代理功能：

当我们访问一个网址，其实nginx会接收到我们的请求，然后由nginx再转发给其他服务器，其中nginx就实现了反向代理的功能，对于客户端来说，并不知道是由哪一台服务器来返回页面的。
### 正向代理和反向代理的区别
http代理可以分为正向代理和反向代理，它们之间的区别主要在于代理的对象不一样，正向代理，代理的对象是客户端，主要是为客户端收发请求，而反向代理，代理的是服务端，主要是为服务端收发请求。