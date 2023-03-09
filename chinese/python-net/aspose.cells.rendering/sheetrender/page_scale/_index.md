---
title: page_scale 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
## page_scale 属性

获取工作表的计算页面比例。
如果设置了 [PageSetup.zoom](/cells/zh/python-net/aspose.cells/pagesetup#zoom)，则返回设置的比例。

### 例子

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
### 定义：
```python
@property
def page_scale(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [SheetRender](/cells/zh/python-net/aspose.cells.rendering/sheetrender)
