---
title: License 构造函数
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells/license/__init__/
is_root: false
---
##  License() {#}
初始化此类的新实例。



```python
def __init__(self):
    ...
```



### 例子

在此示例中，将尝试查找名为 MyLicense.lic 的许可证文件
在包含的文件夹中


组件，在包含调用程序集的文件夹中，
在入口程序集的文件夹中，然后在调用程序集的嵌入式资源中。

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [License](/cells/zh/python-net/aspose.cells/license)
