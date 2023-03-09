---
title: group метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 420
url: /ru/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Сгруппируйте фигуры.


###  Возвращает

Верните форму group.


```python
def group(self, group_items):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| group_items | list | групповые предметы.|
###  Примечания

Фигура в groupItems не должна быть сгруппирована.
Фигура должна быть в этой коллекции фигур.
###  Пример

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
