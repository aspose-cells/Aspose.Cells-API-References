---
title: get_range_by_name method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 120
url: /python-net/aspose.cells/worksheetcollection/get_range_by_name/
is_root: false
---

## get_range_by_name(range_name) {#str}

Gets Range object by pre-defined name.

### Returns 


Range object.


Returns null if the named range does not exist.


```python
def get_range_by_name(self, range_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| range_name | str | Name of range. |


## get_range_by_name(range_name, current_sheet_index, include_table) {#str-int-bool}

Gets [Range](/cells/python-net/aspose.cells/range) by pre-defined name or table's name

### Returns 





```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| range_name | str | Name of range or table's name. |
| current_sheet_index | int | The sheet index. -1 represents global . |
| include_table | bool | Indicates whether checking all tables. |



### See Also
* module [aspose.cells](../../)
* class [WorksheetCollection](/cells/python-net/aspose.cells/worksheetcollection)
