---
title: get_threaded_comments метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells/commentcollection/get_threaded_comments/
is_root: false
---
##  get_threaded_comments(cell_name) {#str}
Получает цепочку комментариев по имени ячейки.


###  Возвращает




```python
def get_threaded_comments(self, cell_name):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| cell_name | str | Имя ячейки.|

###  Примеры

```python

threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
    tc = threadedComments2[i]
    note = tc.notes

```


##  get_threaded_comments(row, column) {#int-int}
Получает цепочку комментариев по индексу строки и столбца.


###  Возвращает




```python
def get_threaded_comments(self, row, column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row | int | Индекс строки.|
| column | int | Индекс столбца.|

###  Примеры

```python

threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
    tc = threadedComments1[i]
    note = tc.notes

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [CommentCollection](/cells/ru/python-net/aspose.cells/commentcollection)
