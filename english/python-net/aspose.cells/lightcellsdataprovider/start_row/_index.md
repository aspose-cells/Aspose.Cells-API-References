---
title: start_row method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 60
url: /python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---

## start_row(row) {#Row}

Starts to save data of one row.



```python
def start_row(self, row):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row | [Row](/cells/python-net/aspose.cells/row) | Row object for implementation to fill data. Its row index is the returned value of latest call of [LightCellsDataProvider.next_row()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>If the row has been initialized in the inner cells model, the existing row object will be used.<br/>Otherwise a temporary Row object will be used for implementation to fill data. |
### Remarks

It will be called at the beginning of saving a row and its cells data.
If current row has some custom properties such as height, style, ...etc.,
implementation should set those properties to given Row object here.


### See Also
* module [aspose.cells](../../)
* class [LightCellsDataProvider](/cells/python-net/aspose.cells/lightcellsdataprovider)
