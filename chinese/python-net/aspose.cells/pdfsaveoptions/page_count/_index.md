---
title: page_count 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 310
url: /zh/python-net/aspose.cells/pdfsaveoptions/page_count/
is_root: false
---
## page_count 属性

获取或设置要保存的页数。

### 评论

默认值为 System.Int32.MaxValue，这意味着将呈现所有页面。

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
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PdfSaveOptions](/cells/zh/python-net/aspose.cells/pdfsaveoptions)
