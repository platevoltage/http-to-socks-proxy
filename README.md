# http-to-socks-proxy
Implements http proxy server which sends requests through the socks proxy (proxies)

## Usage

You can specify proxy or proxyList options. If proxyList is specified, proxy will be selected randomly

```js
var ProxyServer = require('proxy-server');
var options = {
    //proxy: '127.0.0.1:9050',
    proxy: null,
    proxyList: './proxy.list',
    proxyListReloadTimeout: 60 // one minute
};
ProxyServer.createServer(options).listen(8080);
```
