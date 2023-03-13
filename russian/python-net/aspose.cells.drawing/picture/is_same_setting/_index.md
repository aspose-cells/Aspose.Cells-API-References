---
title: is_same_setting метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 140
url: /ru/python-net/aspose.cells.drawing/picture/is_same_setting/
is_root: false
---
##  is_same_setting(obj) {#any}
Возвращает, совпадает ли форма.


###  Возвращает




```python
def is_same_setting(self, obj):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| obj | any |  |

###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
if pic1.is_same_setting(pic1):
    pass
if !pic1.is_same_setting(pic2):
    pass

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
