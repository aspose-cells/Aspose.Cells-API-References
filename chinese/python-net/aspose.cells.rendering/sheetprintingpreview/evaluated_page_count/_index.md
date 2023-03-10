---
title: evaluated_page_count 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---
## evaluated_page_count 属性

评估此工作表的总页数

### 例子

以下代码显示了获取工作表页数的最快方法。

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```
### 定义：
```python
@property
def evaluated_page_count(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [SheetPrintingPreview](/cells/zh/python-net/aspose.cells.rendering/sheetprintingpreview)
