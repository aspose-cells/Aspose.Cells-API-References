---
title: page_index недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 190
url: /ru/python-net/aspose.cells/pptxsaveoptions/page_index/
is_root: false
---
##  page_index недвижимость

Получает или задает отсчитываемый от 0 индекс первой страницы для сохранения.

###  Примечания

По умолчанию 0.

###  Пример

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
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PptxSaveOptions](/cells/ru/python-net/aspose.cells/pptxsaveoptions)
