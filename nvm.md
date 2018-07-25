# 使用nvm管理nodejs
## 安装nvm
> - 安装nvm前，需要卸载以前安装的node.js
> - [下载网址](https://github.com/coreybutler/nvm-windows/releases) 
> - NVM_HOME ：指向nvm安装目录(node.js所有版本都会在这个目录下)
> - NVM_SYMLINK：nodejs安装目录 (当前使用nodejs版本)
> - **注意：nvm不能安装在有空格的目录中**

## 利用nvm安装nodejs
> - [查看可安装的nodejs版本](https://github.com/coreybutler/nodedistro/blob/master/nodeversions.json)
> - nvm install 8.9.1(范例)
```
如果报:Could not retrieve https://nodejs.org/dist/latest/SHASUMS256.txt.
Get https://nodejs.org/dist/latest/SHASUMS256.txt: net/http: TLS handshake timeout
这种错，说明出现远程连接被关闭的问题，这是由于国内网络限制导致的
可以将nvm中node和那npm设置到国内源,在nvm的安装路径下找到settings.txt(如果没有，可新建一个)打开:添加一下代码
node_mirror:npm.taobao.org/mirrors/node/
npm_mirror:npm.taobao.org/mirrors/npm/
```
## 配置npm安装路径
```
1.在node安装路径下建立 node_global 和 node_cache 两个文件夹
2.配置: 例如node安装路径为 D:\nodejs
npm config set prefix "D:\nodejs\node_global
npm config set cache "D:\nodejs\node_cache"
3.配置环境变量
path: D:\nodejs\node_global;
4.配置cnpm
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

## 使用nvm
> - 安装node版本: nvm install 10.6.0 (node版本号)
> - 查看已安装node版本: nvm list
> - 切换node版本: nvm use 10.6.0
> - 卸载node版本: nvm uninstall 10.6.0

## mac安装
