---
title: default_style недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 540
url: /ru/python-net/aspose.cells/workbook/default_style/
is_root: false
---
##  default_style недвижимость

Получает или задает объект книги по умолчанию [Style](/cells/ru/python-net/aspose.cells/style).

###  Примечания

Свойство DefaultStyle полезно для реализации стиля для всей книги.

###  Пример

Следующий код создает и создает новую рабочую книгу и устанавливает для нее значение по умолчанию [Style](/cells/ru/python-net/aspose.cells/style).

```python
from aspose.cells import Workbook

workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle

```
###  Определение:
```python
@property
def default_style(self):
    ...
@default_style.setter
def default_style(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Style](/cells/ru/python-net/aspose.cells/style)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
