---
title: copy_in_range yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 380
url: /tr/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Aralıktaki şekilleri hedef aralığa kopyalayın.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection) | Kaynak şekiller.|
| ca | [CellArea](/cells/tr/python-net/aspose.cells/cellarea) | Kaynak aralığı.|
| dest_row | int | Hedef aralığın hedef satır dizini.|
| dest_column | int | Hedef aralığın hedef sütunu.|
| is_contained | bool | Yalnızca aralıkta bulunan şekillerin kopyalanıp kopyalanmadığı.<br/> Doğruysa, yalnızca aralıktaki şekilleri kopyalar.<br/> Aksi takdirde, MS Office olarak çalışır.|

###  Örnek

```python
from aspose.cells import CellArea

# add a shape
shapes.add_rectangle(2, 0, 2, 0, 130, 130)
area2 = CellArea()
area2.start_column = 1
area2.start_row = 1
area2.end_column = 5
area2.end_row = 11
# copy
shapes.copy_in_range(shapes, area2, 12, 1, False)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
