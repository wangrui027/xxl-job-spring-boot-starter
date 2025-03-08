# xxl-job-spring-boot-starter
## 概述

xxl-job SpringBoot 启动器，开箱即用。引入依赖，配置参数，立即开工，无需手动创建配置类和注入 bean。

本项目源码：[https://github.com/wangrui027/xxl-job-spring-boot-starter](https://github.com/wangrui027/xxl-job-spring-boot-starter)

xxl-job 首页：[https://www.xuxueli.com/xxl-job/](https://www.xuxueli.com/xxl-job/)

xxl-job 源码：[https://github.com/xuxueli/xxl-job/](https://github.com/xuxueli/xxl-job/)

## 使用方式

**1、引入依赖**

```xml
<dependency>
    <groupId>io.github.wangrui027</groupId>
    <artifactId>xxl-job-spring-boot-starter</artifactId>
    <version>2.5.0</version>
</dependency>
```

**2、配置参数**

application.yml 示例：

```yaml
xxl:
  job:
    admin:
      addresses: http://xx.xx.xx.xx:8020/xxl-job-admin
      accessToken: xxx
      timeout: 3
    executor:
      appname: my_app
      address: http://xx.xx.xx.xx:8011
      ip: xx.xx.xx.xx
      port: 8011
      logpath: /data/applogs/xxl-job/jobhandler
      logretentiondays: 30
```

application.properties 示例：

```properties
xxl.job.admin.addresses=http://xx.xx.xx.xx:8020/xxl-job-admin
xxl.job.admin.accessToken=xxx
xxl.job.admin.timeout=3
xxl.job.executor.appname=my_app
xxl.job.executor.address=http://xx.xx.xx.xx:8011
xxl.job.executor.ip=xx.xx.xx.xx
xxl.job.executor.port=8011
xxl.job.executor.logpath=/data/applogs/xxl-job/jobhandler
xxl.job.executor.logretentiondays=30
```

## 鸣谢

感谢**徐雪里**同学为我们带来 `xxl-job` 这么简单好用的分布式任务调度平台。
