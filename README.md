# fis-startup-for-xiaowei

## 环境安装

### 安装node环境

下载地址：https://nodejs.org/en/download/
版本要求： `>0.8`

### 安装fis3

```
npm install -g fis3
```

## 版本控制

完成两件事情：（demo代码在这里下载 https://github.com/chyingp/fis-startup-for-xiaowei）
1. 从源码目录同步到发布目录
2. 版本控制

首先，配置文件`fis-conf.js`声明如下配置

```
// js、css、png都加上md5
fis.match('*.{js,css,png}', {
  useHash: true
});
```

然后，运行下面命令。`output`命令可以自己指定。然后看下生成的文件，应该就木有问题了。

```
fis3 release -d ../output
```


