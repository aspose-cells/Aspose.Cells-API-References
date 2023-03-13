---
title: page_scale недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 90
url: /ru/python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---
##  page_scale недвижимость

Получает рассчитанный масштаб страницы листа.
Возвращает заданный масштаб, если установлено значение [PageSetup.zoom](/cells/ru/python-net/aspose.cells/pagesetup#zoom). В противном случае возвращает рассчитанный масштаб в соответствии с [PageSetup.fit_to_pages_wide](/cells/ru/python-net/aspose.cells/pagesetup#fit_to_pages_wide) и [PageSetup.fit_to_pages_tall](/cells/ru/python-net/aspose.cells/pagesetup#fit_to_pages_tall).

###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```
###  Определение:
```python
@property
def page_scale(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.rendering](../../)
* класс [SheetRender](/cells/ru/python-net/aspose.cells.rendering/sheetrender)
