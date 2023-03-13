---
title: add_identify метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Устанавливает, какую метку элемента в каждом поле страницы использовать для идентификации диапазона данных.
Значение pageItemIndex.Length должно быть равно PageFieldCount, поэтому сначала добавьте поле страницы.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range_index | int |Индекс диапазона данных консолидации.|
| page_item_index | list | Индекс элемента страницы в поле каждой страницы.<br/>pageItemIndex[2] = 1 означает, что второй элемент в третьем поле используется для идентификации этого диапазона.<br/> pageItemIndex[1] = -1 означает, что во втором поле нет элемента, который можно использовать для идентификации этого диапазона.<br/> и MS автоматически создаст «пустой» элемент во втором поле, чтобы идентифицировать этот диапазон.|



###  Смотрите также
* модуль [aspose.cells.pivot](../../)
* класс [PivotPageFields](/cells/ru/python-net/aspose.cells.pivot/pivotpagefields)
