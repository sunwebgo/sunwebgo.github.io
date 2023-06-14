# 基于Hexo框架和Fluid主题实现的静态博客站点
网站地址：https://xhablog.online
Hexo官网：https://hexo.io/
Fluid主题用户手册：https://fluid-dev.github.io/hexo-fluid-docs/start/

# 1.安装前的环境准备

1. **本机nodejs环境**

打开dos命令窗口，查看本机nodejs版本

```ini
node -v
```

2. **本机git环境**

打开git客户端，查看git版本

![image-20230608150301551](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608150301551.png)

3. **本机npm、cnpm环境**

```ini
npm -v
cnpm -v
```

![image-20230608150704760](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608150704760.png)



# 2.安装hexo

1. **hexo官网**

[Hexo](https://hexo.io/zh-cn/index.html)

2. **安装hexo**

在dos命令下安装hexo

```ini
npm install hexo-cli -g
```

3. **初始化博客**

在本地创建文件夹，用于存储hexo数据

![image-20230608151204035](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608151204035.png)

在此目录下打开git客户端，初始化hexo

```ini
hexo init
```

![image-20230608151412056](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608151412056.png)

就会从github当中克隆对应的项目，文件夹初始化如下：

<img src="https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608151648168.png" alt="image-20230608151648168" style="zoom: 67%;" />

4. **启动博客**

在此目录下打开git客户端，执行以下命令

```ini
hexo server
```

![image-20230608151811450](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608151811450.png)

访问本机4000端口

![image-20230608151847006](https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608151847006.png)

5. **更新hexo版本**

```ini
npm update hexo -g
```

6. **卸载hexo**

```ini
npm uninstall hexo-cli -g
```



# 3.关于页的创建

### 创建关于页

首次使用主题的「关于页」需要手动在Hexo工程目录下执行以下命令：

```bash
$ hexo new page about
```

创建成功后修改 `/source/about/index.md`，添加 `layout` 属性。

修改后的文件示例如下：

```yaml
---
title: 标题
layout: about
---

这里可以写正文，支持 Markdown, HTML
```

WARNING

`layout: about` 必须存在，并且不能修改成其他值，否则不会显示头像等样式。



# 4.安装主题出现的问题

安装主题后如果出现以下问题

<img src="https://imagebed-xuhuaiang.oss-cn-shanghai.aliyuncs.com/typora/image-20230608172302075.png" alt="image-20230608172302075" style="zoom:67%;" />

使用以下命令解决

```ini
npm install css --save
```



