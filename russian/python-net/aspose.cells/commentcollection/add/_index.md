---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
Добавляет комментарий к коллекции.


###  Возвращает

[Comment](/cells/ru/python-net/aspose.cells/comment) индекс объекта.


```python
def add(self, cell_name):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| cell_name | str | Cell имя.|

###  Примеры

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
Добавляет комментарий к коллекции.


###  Возвращает

[Comment](/cells/ru/python-net/aspose.cells/comment) индекс объекта.


```python
def add(self, row, column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row | int | Cell индекс строки.|
| column | int | Cell индекс столбца.|

###  Примеры

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Comment](/cells/ru/python-net/aspose.cells/comment)
* класс [CommentCollection](/cells/ru/python-net/aspose.cells/commentcollection)
