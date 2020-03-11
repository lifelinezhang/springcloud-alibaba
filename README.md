# nacos
这里使用的是官方推荐的1.1.4版本`https://github.com/alibaba/nacos/releases/tag/1.1.4`，下载完之后解压，然后
```
cd nacos/
mvn -Prelease-nacos -Dmaven.test.skip=true clean install -U 
```
等到所有的包都success之后，将`nacos-1.1.4\distribution\target\nacos-server-1.1.4\nacos\target`文件中的nacos-server.jar包复制到`nacos-1.1.4\distribution\target`中，然后双击`nacos-1.1.4\distribution\bin`中的startup.cmd，就可以启动了。此时访问`http://localhost:8848/nacos`就可以跳转到登录界面了。默认账密： nacos/nacos
