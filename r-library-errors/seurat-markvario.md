---
description: >-
  Error: package or namespace load failed for ‘Seurat’: object ‘markvario’ is
  not exported by 'namespace:spatstat'
---

# Seurat-markvario

{% embed url="https://github.com/satijalab/seurat/issues/4226" %}

Seurat依赖的R包`spatstat`升级了，把原来的函数`spatstat::markvario` 变成了 `spatstat.core::markvario`

这是一个分析空间数据的R包，在Seurat中是分析空间转录组数据的支持包，对应的主要函数是`Seurat::RunMarkVario()`

* **SOLVING**: 安装旧版本的spatstat

```
remove.packages(grep("spatstat", installed.packages(), value = T))
.rs.restartR()
devtools::install_version("spatstat", version = "1.64-1")^
```
