原版仓库：https://github.com/yongjiu8/unidbg-jd-sign

unidbg线程不安全，原版有问题。根据unidbg示例代码，稍微修改了一下。

已打Docker：https://hub.docker.com/r/zhx47/jd_sign
### 打jar包
配置好maven环境的前提下，项目主目录执行
````java
 mvn clean package -Dmaven.test.skip=true  
````
使用maven的package即可，之后会发现生成一个target目录其中里面就有jar包了。
```
mvn package
```

把application.properties 复制到 jar包所在目录 方便修改

### 使用jar包
```
java -jar unidbg-server-1.0.0.jar 
```

