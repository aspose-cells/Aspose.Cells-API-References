---
title: add_identify method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---

## add_identify(range_index, page_item_index) {#int-list}

Sets which item label in each page field to use to identify the data range.
The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| range_index | int | The consolidation data range index. |
| page_item_index | list | The page item index in the each page field.<br/>pageItemIndex[2] = 1 means the second item in the third field to use to identify this range.<br/>pageItemIndex[1] = -1 means no item in the second field to use to identify this range <br/>and MS will auto create "blank" item in the second field  to identify this range. |



### See Also
* module [aspose.cells.pivot](../../)
* class [PivotPageFields](/cells/python-net/aspose.cells.pivot/pivotpagefields)
