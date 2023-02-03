---
title: create_safe_sheet_name method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---

## create_safe_sheet_name(name_proposal) {#str}

Checks given sheet name and create a valid one when needed.
If given sheet name conforms to the rules of excel sheet name, then return it.
Otherwise string will be truncated if length exceeds the limit
and invalid characters will be replaced with ' ', then return the rebuilt string value.


### Returns 





```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| name_proposal | str | sheet name to be used |


## create_safe_sheet_name(name_proposal, replace_char) {#str-char}

Checks given sheet name and create a valid one when needed.
If given sheet name conforms to the rules of excel sheet name, then return it.
Otherwise string will be truncated if length exceeds the limit
and invalid characters will be replaced with given character, then return the rebuilt string value.


### Returns 





```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| name_proposal | str | sheet name to be used |
| replace_char | char | character which will be used to replace invalid characters in given sheet name |



### See Also
* module [aspose.cells](../../)
* class [CellsHelper](/cells/python-net/aspose.cells/cellshelper)
