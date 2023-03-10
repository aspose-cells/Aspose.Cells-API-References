---
title: custom_document_properties 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 270
url: /zh/python-net/aspose.cells/worksheetcollection/custom_document_properties/
is_root: false
---
## custom_document_properties 属性

返回代表电子表格所有自定义文档属性的 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 集合。

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
workbook.worksheets.custom_document_properties.add("Checked by", "Jane")

```
### 定义：
```python
@property
def custom_document_properties(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CustomDocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection)
* 类 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty)
* 类 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection)
