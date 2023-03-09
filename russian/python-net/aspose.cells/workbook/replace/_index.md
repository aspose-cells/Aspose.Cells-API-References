---
title: replace метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 330
url: /ru/python-net/aspose.cells/workbook/replace/
is_root: false
---
##  replace(place_holder, new_value) {#str-str}
Заменяет значение ячейки новой строкой.



```python
def replace(self, place_holder, new_value):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_value | str | Строковое значение для замены|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


##  replace(place_holder, new_value) {#str-int}
Заменяет значение ячейки новым целым числом.



```python
def replace(self, place_holder, new_value):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_value | int | Целое значение для замены|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


##  replace(place_holder, new_value) {#str-float}
Заменяет значение ячейки новым двойным значением.



```python
def replace(self, place_holder, new_value):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_value | float | Двойное значение для замены|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


##  replace(bool_value, new_value) {#bool-any}
Заменяет значения ячеек новыми данными.



```python
def replace(self, bool_value, new_value):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| bool_value | bool | Логическое значение, которое необходимо заменить.|
| new_value | any | Новое значение. Может быть строкой, целым числом, двойным значением или значением DateTime.|


##  replace(int_value, new_value) {#int-any}
Заменяет значения ячеек новыми данными.



```python
def replace(self, int_value, new_value):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| int_value | int | Заменяемое целочисленное значение.|
| new_value | any | Новое значение. Может быть строкой, целым числом, двойным значением или значением DateTime.|


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Заменяет значение ячейки новым массивом строк.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_values | list | Массив строк для замены|
| is_vertical | bool | Правда-вертикально, ложно-горизонтально|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Заменяет значения ячеек целочисленным массивом.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_values | list | Целочисленный массив для замены|
| is_vertical | bool | Правда-вертикально, ложно-горизонтально|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
Заменяет значения ячеек двойным массивом.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_values | list | Двойной массив для замены|
| is_vertical | bool | Правда-вертикально, ложно-горизонтально|

###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_value, options) {#str-str-ReplaceOptions}
Заменяет значение ячейки новой строкой.



```python
def replace(self, place_holder, new_value, options):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| place_holder | str | Cell заполнитель|
| new_value | str | Строковое значение для замены|
| options | [ReplaceOptions](/cells/ru/python-net/aspose.cells/replaceoptions) | Варианты замены|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
