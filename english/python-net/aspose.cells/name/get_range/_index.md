---
title: get_range method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/name/get_range/
is_root: false
---

## get_range() {#}

Gets the range if this name refers to a range.

### Returns 


The range.


```python
def get_range(self):
    ...
```




## get_range(recalculate) {#bool}

Gets the range if this name refers to a range

### Returns 


The range.


```python
def get_range(self, recalculate):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| recalculate | bool | whether recalculate it if this name has been calculated before this invocation. |


## get_range(sheet_index, row, column) {#int-int-int}

Gets the range if this name refers to a range.
If the reference of this name is not absolute, the range may be different for different cell.

### Returns 


The range.


```python
def get_range(self, sheet_index, row, column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| sheet_index | int | The according sheet index. |
| row | int | The according row index. |
| column | int | The according column index |



### See Also
* module [aspose.cells](../../)
* class [Name](/cells/python-net/aspose.cells/name)
