---
title: printing_page_type недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 210
url: /ru/python-net/aspose.cells/paginatedsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type недвижимость

Указывает, какие страницы не будут распечатаны.

###  Примечания

Если содержимое на листе разрежено, некоторые страницы будут полностью пустыми в выходном файле PDF.
Если вам не нужны эти пустые страницы, вы можете использовать эту опцию, чтобы опустить их.

###  Примеры

Следующий код пропускает пустые страницы или страницы, которые содержат только некоторое содержимое стиля, такое как фон ячейки, границы.

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
###  Определение:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PaginatedSaveOptions](/cells/ru/python-net/aspose.cells/paginatedsaveoptions)
* класс [PrintingPageType](/cells/ru/python-net/aspose.cells/printingpagetype)
