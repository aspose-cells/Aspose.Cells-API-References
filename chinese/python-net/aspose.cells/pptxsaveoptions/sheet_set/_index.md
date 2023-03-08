---
title: sheet_set 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 240
url: /zh/python-net/aspose.cells/pptxsaveoptions/sheet_set/
is_root: false
---
## sheet_set 属性

获取或设置要呈现的工作表。默认为工作簿中的所有可见工作表：[SheetSet.visible](/cells/zh/python-net/aspose.cells.rendering/sheetset#visible)。

### 例子

以下代码仅将活动工作表呈现为 pdf。

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import SheetSet

workbook = Workbook("Book1.xlsx")
activeSheetIndex = workbook.worksheets.active_sheet_index
pdfSaveOptions = PdfSaveOptions()
# set active sheet index to sheet set.
pdfSaveOptions.sheet_set = SheetSet([activeSheetIndex])
workbook.save("output.pdf", pdfSaveOptions)

```
### 定义：
```python
@property
def sheet_set(self):
    ...
@sheet_set.setter
def sheet_set(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PptxSaveOptions](/cells/zh/python-net/aspose.cells/pptxsaveoptions)
* 类 [SheetSet](/cells/zh/python-net/aspose.cells.rendering/sheetset)
