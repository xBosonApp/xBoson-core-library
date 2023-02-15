# xBoson 平台 jar 库

因为以下原因创建了这个库:

1. jar库没有上传到 Maven 中.
2. 库版本冲突, 需要人工调整.
3. 库升级失败后进行回滚.

该项目由 [上海竹呗信息技术有限公司](https://xboson.net/) 提供技术支持.


## 注意

hadoop 必须用 hadoop-common-3.1.3-with-dependencies.jar 否则报错: No FileSystem for scheme "hdfs" 


## 下载依赖

`mvn dependency:copy-dependencies`


## 目录说明

* xboson-war - xboson 主项目 WEB-INF/lib 中的文件
* xboson-jar - xboson 主项目 libs 目录备份
* local-jar  - 这些文件在互联网仓库中不存在
* target     - 通过配置脚本从 mvn 仓库中拉取的文件


## TODO

下载文件后部署在正确的目录.


## 其他

* [xBoson平台运算核心](https://github.com/yanmingsohu/xBoson-core)