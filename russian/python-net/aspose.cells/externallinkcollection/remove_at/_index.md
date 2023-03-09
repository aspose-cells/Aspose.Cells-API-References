---
title: remove_at метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Удаляет указанную внешнюю ссылку из книги.



```python
def remove_at(self, index):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| index | int | индекс внешней ссылки, которую необходимо удалить.|
###  Примечания

При удалении внешней ссылки все формулы, ссылающиеся на нее, также будут удалены, поскольку
ссылки становятся недействительными.

##  remove_at(index, update_references_as_local) {#int-bool}
Удаляет указанную внешнюю ссылку из книги.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| index | int | индекс внешней ссылки, которую необходимо удалить.|
| update_references_as_local | bool | Обновлять ли все ссылки данной внешней ссылки на ссылку самой текущей книги.|
###  Примечания

Если требуется обновить ссылки, ссылки на внешние ссылки в формулах будут заменены на текущую книгу.
Например, внешняя ссылка, которую нужно удалить, называется «externalsource.xlam», и она определяет одну пользовательскую функцию «customfunction()»,
исходная формула одной ячейки: "='externalsource.xlam'!customfunction()",
после удаления формула станет "=customfunction()".
Если ссылку обновлять не требуется, все формулы со ссылкой на эту внешнюю ссылку
также будут удалены, потому что эти ссылки станут недействительными.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [ExternalLinkCollection](/cells/ru/python-net/aspose.cells/externallinkcollection)
