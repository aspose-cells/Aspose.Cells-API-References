---
title: printing_page_type 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 210
url: /zh/python-net/aspose.cells/pptxsaveoptions/printing_page_type/
is_root: false
---
## printing_page_type 属性

指示将不打印哪些页面。

### 评论

如果工作表中的内容稀疏，则输出的 pdf 文件中会有一些页面完全空白。
如果你不想要这些空白页，你可以使用这个选项来忽略它们。

### 例子

以下代码省略了空白页面或仅包含一些样式内容（如单元格背景、边框）的页面。

```python
from aspose.cells import PdfSaveOptions, PrintingPageType, Workbook

wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# ignore blank pages
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_BLANK
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions)
# ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_STYLE
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions)

```
### 定义：
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PptxSaveOptions](/cells/zh/python-net/aspose.cells/pptxsaveoptions)
* 类 [PrintingPageType](/cells/zh/python-net/aspose.cells/printingpagetype)
