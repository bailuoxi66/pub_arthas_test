# 1、学习使用

## 1.1 arhtas插件安装

打开idea-》右上角Intelli IDEA-》Preferences-》Plugins-》MarketPlace-》输入arthas-》点击install-》Restart IDEA

<img src="/Users/luoyu/Library/Application Support/typora-user-images/image-20210111112550605.png" alt="image-20210111112550605" style="zoom:50%;" />

如上图：arthas安装成功后，找一个方法名或者其他，右键，看到Arthas Command，点击Trace，得到如下结果

```java
trace com.example.Client main -v -n 5 --skipJDKMethod false '1==1'
```

所以，整体来说就是构造arthas的命令行，使得使用起来更加简单

## 1.2 arhtas相关文档

<img src="/Users/luoyu/Library/Application Support/typora-user-images/image-20210111120430506.png" alt="image-20210111120430506" style="zoom:50%;" />

链接如下：https://arthas.aliyun.com/doc/advanced-use.html

如上同理：可以找打arthas plugin文档：点击Arthas Idea Plugin Help

<img src="/Users/luoyu/Library/Application Support/typora-user-images/image-20210111120943376.png" alt="image-20210111120943376" style="zoom:20%;" />

https://github.com/WangJi92/arthas-idea-plugin/blob/master/README.md

https://plugins.jetbrains.com/plugin/13581-arthas-idea

## 1.3 arthas安装

方法一：https://arthas.aliyun.com/doc/install-detail.html

方法二：

```java
curl -sk https://arthas.aliyun.com/arthas-boot.jar -o ~/.arthas-boot.jar  && echo "alias as.sh='java -jar ~/.arthas-boot.jar --repo-mirror aliyun --use-http 2>&1'" >> ~/.bashrc && source ~/.bashrc && echo "source ~/.bashrc" >> ~/.bash_profile && source ~/.bash_profile
```

## 1.4 watch、trace和rest插件

### 1.4.1 安装rest插件

![image-20210113011056222](/Users/luoyu/Library/Application Support/typora-user-images/image-20210113011056222.png)

![image-20210113011142366](/Users/luoyu/Library/Application Support/typora-user-images/image-20210113011142366.png)

观察trace

- 启动服务arthas-plugin-demo
- 启动arthas服务
- ![image-20210113011327319](/Users/luoyu/Library/Application Support/typora-user-images/image-20210113011327319.png)

### 1.4.2 Trace:

![image-20210113011627600](/Users/luoyu/Library/Application Support/typora-user-images/image-20210113011627600.png)

### 1.4.3 Watch：

<img src="/Users/luoyu/Library/Application Support/typora-user-images/image-20210113011737361.png" alt="image-20210113011737361" style="zoom:50%;" />