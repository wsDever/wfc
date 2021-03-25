#### 安装工具、生成插件结构

``` javascript
npm install -g yo generator-code
```
``` javascript
yo code
```

``` javascript
code [progress-name]
```
#### 调试
press `F5` 

#### 发布插件

 - 安装vsce

``` javascript
npm install -g vsce
```

 - 创建[publisher](https://marketplace.visualstudio.com/manage/publishers/wushang)
 - 在package.json中配置publisher，设置值为上面创建。
 - 生成[access Token](https://dev.azure.com/809663381/_usersSettings/tokens)
 - 打包
  
``` javascript
vsce package
```
 - 输入access Token， 打包成功。

#### 发布、更新、删除插件

``` javascript
vsce publish
```

``` javascript
vsce publish [2.0.1]
```

``` javascript
vsce unpublish (publisher name).(extension name)
```

#### 参考文档

 - [中文文档](https://liiked.github.io/VS-Code-Extension-Doc-ZH/#/working-with-extensions/publish-extension)
 - [英文文档](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
 - [问题处理](https://www.jianshu.com/p/c75d0897e878)
 - [问题处理](https://blog.werner.wiki/how-to-open-recaptcha/)

