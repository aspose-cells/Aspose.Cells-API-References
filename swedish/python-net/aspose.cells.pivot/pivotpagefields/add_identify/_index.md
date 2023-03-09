---
title: add_identify metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Ställer in vilken objektetikett i varje sidfält som ska användas för att identifiera dataintervallet.
pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| range_index | int | Konsolideringsdataintervallsindex.|
| page_item_index | list | Sidobjektets index i varje sidfält.<br/>pageItemIndex[2] = 1 betyder det andra objektet i det tredje fältet som ska användas för att identifiera detta intervall.<br/> pageItemIndex[1] = -1 betyder inget objekt i det andra fältet att använda för att identifiera detta intervall<br/> och MS kommer automatiskt att skapa "tomt" objekt i det andra fältet för att identifiera detta intervall.|



###  Se även
* modul [aspose.cells.pivot](../../)
* klass [PivotPageFields](/cells/sv/python-net/aspose.cells.pivot/pivotpagefields)
