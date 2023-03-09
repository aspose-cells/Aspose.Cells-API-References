---
title: ungroup метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 450
url: /ru/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
Разгруппирует элементы формы.



```python
def ungroup(self, group):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| group | [GroupShape](/cells/ru/python-net/aspose.cells.drawing/groupshape) | Форма группы.|
###  Примечания

Если фигура группы сгруппирована другой фигурой группы, ничего не будет сделано.
###  Пример


```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# group
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)
# ungroup
shapes.ungroup(groupShape)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
