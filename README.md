# 构建脚本

## 介绍

主要由三个配置脚本组成，分别是

- `app.gradle` 完成 `app` 模块配置
- `module.gradle` 完成 `module` 模块配置
- `project.gradle` 完成 `project` 级别配置

## 使用

详细可以参考 `project/` 中的例子


### `app` 使用

```gradle
ext.params = [
        applicationId : "com.zfy.mantis.sample",
        resourcePrefix: "index_"
]
apply from: '../scripts/app.gradle'
```

### `module` 使用

```gradle
apply from: '../scripts/module.gradle'
```

### `project` 使用

```gradle
apply from: "scripts/project.gradle"
```