---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.drawing/textboxcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width) {#int-int-int-int}
Добавляет текстовое поле в коллекцию.


###  Возвращает

[TextBox](/cells/ru/python-net/aspose.cells.drawing/textbox) индекс объекта.


```python
def add(self, upper_left_row, upper_left_column, height, width):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int |Индекс левого верхнего столбца.|
| height | int | Высота текстового поля в пикселях.|
| width | int | Ширина текстового поля в пикселях.|

###  Пример

```python

# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [TextBox](/cells/ru/python-net/aspose.cells.drawing/textbox)
* класс [TextBoxCollection](/cells/ru/python-net/aspose.cells.drawing/textboxcollection)
