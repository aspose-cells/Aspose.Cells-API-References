---
title: create_safe_sheet_name метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 90
url: /ru/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Проверяет заданное имя листа и при необходимости создает допустимое.
Если данное имя листа соответствует правилам имени листа Excel, верните его.
В противном случае строка будет усечена, если длина превысит лимит
и недопустимые символы будут заменены на ' ', а затем вернут перестроенное строковое значение.


###  Возвращает




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| name_proposal | str | имя листа, которое будет использоваться|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Проверяет заданное имя листа и при необходимости создает допустимое.
Если данное имя листа соответствует правилам имени листа Excel, верните его.
В противном случае строка будет усечена, если длина превысит лимит
и недопустимые символы будут заменены заданным символом, а затем вернут перестроенное строковое значение.


###  Возвращает




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| name_proposal | str | имя листа, которое будет использоваться|
| replace_char | char | символ, который будет использоваться для замены недопустимых символов в заданном имени листа|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [CellsHelper](/cells/ru/python-net/aspose.cells/cellshelper)
