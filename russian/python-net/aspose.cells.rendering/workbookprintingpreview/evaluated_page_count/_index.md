---
title: evaluated_page_count недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---
##  evaluated_page_count недвижимость

Оцените общее количество страниц в этой книге

###  Пример

В следующем коде показан самый быстрый способ получить количество страниц книги.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```
###  Определение:
```python
@property
def evaluated_page_count(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.rendering](../../)
* класс [WorkbookPrintingPreview](/cells/ru/python-net/aspose.cells.rendering/workbookprintingpreview)
