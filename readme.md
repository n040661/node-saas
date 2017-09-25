node-sass 安装

npm ERR! node v5.2.0
npm ERR! npm  v3.3.12
npm ERR! code ELIFECYCLE

npm ERR! node-sass@3.8.0 postinstall: `node scripts/build.js`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the node-sass@3.8.0 postinstall script 'node scripts/build.js'.
npm ERR! Make sure you have the latest version of node.js and npm installed.
npm ERR! If you do, this is most likely a problem with the node-sass package,
npm ERR! not with npm itself.
npm ERR! Tell the author that this fails on your system:
npm ERR!     node scripts/build.js
npm ERR! You can get their info via:
npm ERR!     npm owner ls node-sass
npm ERR! There is likely additional logging output above.

npm ERR! Please include the following file with any support request:
npm ERR!     K:\vuejs\my-project\npm-debug.log


解决方法1：
别的项目里拷贝node-sass

后提示：ERROR in Cannot find module 'lodash.clonedeep'；

npm i lodash.assign (百度了下，看到说要下载这个，也不知道是啥玩意儿)OK了

但是还是不知道哪个报错啥原因。。。

 

解决方法2：

cnpm下载node-sass失败解决方法:
可能由于网络问题下载win32-x64-47_binding.node失败,去https://github.com/sass/node-...这里下载需要的版本
下载后放到某目录下,如我的放到D盘根目录
1执行命令: set SASS_BINARY_PATH=D:win32-x64-47_binding.node
2安装node-sass: cnpm i node-sass
3安装node-sass成功后继续执行cnpm i下载其他依赖即可

npm install cnpm

cnpm install node-sass