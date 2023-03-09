---
title: page_count недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells/xpssaveoptions/page_count/
is_root: false
---
##  page_count недвижимость

Получает или задает количество страниц для сохранения.

###  Примечания

По умолчанию используется System.Int32.MaxValue, что означает, что будут отображаться все страницы.

###  Примеры

В следующем примере показано, как преобразовать диапазон страниц (3 и 4) в файле Excel Microsoft в PDF.

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
###  Определение:
```python
@property
def page_count(self):
    ...
@page_count.setter
def page_count(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [XpsSaveOptions](/cells/ru/python-net/aspose.cells/xpssaveoptions)
