---
title: start_cell method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/aspose.cells/lightcellsdataprovider/start_cell/
is_root: false
---

## start_cell(cell) {#Cell}

Starts to save data of one cell.



```python
def start_cell(self, cell):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell | [Cell](/cells/python-net/aspose.cells/cell) | Cell object for implementation to fill data. Its column index is the returned value of latest call of [LightCellsDataProvider.next_cell()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_cell).<br/>If the cell has been initialized in the inner cells model, the existed cell object will be used.<br/>Otherwise a temporary Cell object will be used for implementation to fill data. |
### Remarks




### See Also
* module [aspose.cells](../../)
* class [LightCellsDataProvider](/cells/python-net/aspose.cells/lightcellsdataprovider)
