---
title: License类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 980
url: /zh/python-net/aspose.cells/license/
is_root: false
---
## License类
提供许可组件的方法。



License 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [License()](/cells/zh/python-net/aspose.cells/license/__init__/#) |初始化此类的新实例。|


### 方法
|方法|描述|
| :- | :- |
| [set_license(license_name)](/cells/zh/python-net/aspose.cells/license/set_license/#str) |许可组件。|
| [set_license(stream)](/cells/zh/python-net/aspose.cells/license/set_license/#io.RawIOBase) |许可组件。|



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
* 模块 [aspose.cells](..)
