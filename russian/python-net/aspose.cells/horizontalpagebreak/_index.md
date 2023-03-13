---
title: HorizontalPageBreak класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 750
url: /ru/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak класс
Инкапсулирует объект, представляющий горизонтальный разрыв страницы.



Тип HorizontalPageBreak предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [start_column](/cells/ru/python-net/aspose.cells/horizontalpagebreak/start_column) | Получает индекс начального столбца этого горизонтального разрыва страницы.|
| [end_column](/cells/ru/python-net/aspose.cells/horizontalpagebreak/end_column) | Получает индекс конечного столбца этого горизонтального разрыва страницы.|
| [row](/cells/ru/python-net/aspose.cells/horizontalpagebreak/row) | Получает индекс строки, отсчитываемый от нуля.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Смотрите также
* модуль [aspose.cells](..)
