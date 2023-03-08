---
title: evaluated_page_count 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
## evaluated_page_count 属性

评估此工作簿的总页数

### 例子

以下代码显示了获取工作簿页数的最快方法。

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
### 定义：
```python
@property
def evaluated_page_count(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [WorkbookPrintingPreview](/cells/zh/python-net/aspose.cells.rendering/workbookprintingpreview)
