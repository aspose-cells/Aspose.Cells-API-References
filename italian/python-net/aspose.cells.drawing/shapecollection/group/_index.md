---
title: metodo group
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 420
url: /it/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Raggruppa le forme.


###  ritorna

Restituisci la forma group.


```python
def group(self, group_items):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| group_items | list | gli elementi del gruppo.|
###  Osservazioni

La forma in groupItems non deve essere raggruppata.
La forma deve essere in questa raccolta Shapes.
###  Esempio

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
