---
title: page_index 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells/pptxsaveoptions/page_index/
is_root: false
---
## page_index 属性

获取或设置要保存的第一个页面的从 0 开始的索引。

### 评论

默认为 0。

### 例子

以下示例显示如何将 Microsoft Excel 文件中的一系列页面（3 和 4）呈现为 PDF。

```python
from aspose.cells import PdfSaveOptions, Workbook

# Open an Excel file
wb = Workbook("Book1.xlsx")
options = PdfSaveOptions()
# Print only Page 3 and Page 4 in the output PDF
# Starting page index (0-based index)
options.page_index = 3
# Number of pages to be printed
options.page_count = 2
# Save the PDF file
wb.save("output.pdf", options)

```
### 定义：
```python
@property
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PptxSaveOptions](/cells/zh/python-net/aspose.cells/pptxsaveoptions)
