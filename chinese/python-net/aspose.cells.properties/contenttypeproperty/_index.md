---
title: ContentTypeProperty类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
## ContentTypeProperty类
表示标识符信息。



ContentTypeProperty 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [name](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty/name) |返回或设置对象的名称。|
| [value](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty/value) |返回或设置内容类型属性的值。|
| [type](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty/type) |获取和设置属性的类型。|
| [is_nillable](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) |指示该值是否可以为空。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells.properties](..)
