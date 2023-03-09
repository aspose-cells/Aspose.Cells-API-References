---
title: region 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 520
url: /zh/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
## region 属性

获取或设置工作簿的区域设置。

### 评论

1. Aspose.Cells 组件用于从模板文件加载的工作簿的区域设置：
i). 对于 XLS 文件，有为区域设置定义的字段，MS Excel 在保存 XLS 文件时确实将区域设置数据保存到文件中。
因此，我们使用工作簿模板文件中保存的 region。
如果您不想使用保存在XLS文件中的region，请在加载模板文件后将其重置为预期的（如CountryCode.Default）。
并且，我们在保存 XLS 文件时也将用户指定的值（通过这种方法）保存到文件中。
ii). 对于其他文件格式，如XLSX、XLSB...等，文件格式规范中没有定义区域设置字段。
因此，我们为工作簿使用应用程序环境的区域设置。
并且，无法为具有这些文件格式的生成文件保留用户指定的值（通过此方法）。
2、在MS Excel中查看效果：
此处应用的区域设置只能在运行时使用 Aspose.Cells 组件生效，而不是在使用 MS Excel 查看生成的文件时生效。
即使是保存了指定区域设置数据的生成的 XLS 文件，使用 MS Excel 查看/编辑时，
用于MS Excel格式化的region始终是MS Excel运行环境的默认区域设置，
不是保存在文件中的那个。
### 定义：
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CountryCode](/cells/zh/python-net/aspose.cells/countrycode)
* 类 [WorkbookSettings](/cells/zh/python-net/aspose.cells/workbooksettings)
