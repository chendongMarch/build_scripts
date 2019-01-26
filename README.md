# 构建脚本

## 介绍

主要由三个配置脚本组成，分别是

- script/app.gradle 完成 application 模块配置
- script/module.gradle 完成 module 模块配置
- script/project.gradle 完成 project 级别配置


## 使用

`app/build.gradle` 使用

```gradle
ext.params = [
        applicationId : "com.zfy.mantis.sample",
        resourcePrefix: "index_"
]
apply from: '../scripts/app.gradle'
```

`module/build.gradle` 使用

```gradle
apply from: '../scripts/module.gradle'
```

`project/build.gradle` 使用

```gradle
apply from: "scripts/project.gradle"
```