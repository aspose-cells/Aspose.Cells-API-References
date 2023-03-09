---
title: delete_rows метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 260
url: /ru/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Удаляет несколько строк.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_index | int |Индекс первой строки, который необходимо удалить.|
| total_rows | int | Количество строк, которые необходимо удалить.|
###  Примечания

Если удаленный диапазон содержит верхнюю часть (не всю) таблицы (ListObject),
диапазон не может быть удален, и ничего не будет сделано. Он работает как MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Удаляет несколько строк на листе.


###  Возвращает




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row_index | int | Индекс строки.|
| total_rows | int | Количество строк, которые необходимо удалить.|
| update_reference | bool | Указывает, обновляются ли ссылки на других листах.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
