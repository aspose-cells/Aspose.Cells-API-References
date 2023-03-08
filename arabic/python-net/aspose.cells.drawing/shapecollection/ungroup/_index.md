---
title: طريقة ungroup
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 450
url: /ar/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
يفك تجميع عناصر الشكل.



```python
def ungroup(self, group):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| group | [GroupShape](/cells/ar/python-net/aspose.cells.drawing/groupshape) | شكل المجموعة.|
###  ملاحظات

إذا تم تجميع شكل المجموعة بواسطة شكل مجموعة آخر ، فلن يتم فعل أي شيء.
###  مثال


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



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
