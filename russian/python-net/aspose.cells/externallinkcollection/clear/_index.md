---
title: clear метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Удаляет все внешние ссылки.



```python
def clear(self):
    ...
```


###  Примечания

При удалении внешних ссылок все формулы, которые ссылаются на них, также будут удалены, потому что
ссылки становятся недействительными.

##  clear(update_references_as_local) {#bool}
Удаляет все внешние ссылки.



```python
def clear(self, update_references_as_local):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| update_references_as_local | bool | Обновлять ли все ссылки на внешние ссылки как ссылки на текущую книгу.|
###  Примечания

Если требуется обновить ссылки, ссылки на внешние ссылки в формулах будут заменены на текущую книгу.
Например, исходная формула одной ячейки: "='externalsource.xlam'!customfunction()",
после удаления внешних ссылок формула станет "=customfunction()".
Если ссылки обновлять не требуется, все формулы со ссылками на внешние ссылки
также будут удалены, потому что эти ссылки станут недействительными.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [ExternalLinkCollection](/cells/ru/python-net/aspose.cells/externallinkcollection)
