---
title: delete_rows method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 260
url: /python-net/aspose.cells/cells/delete_rows/
is_root: false
---

## delete_rows(row_index, total_rows) {#int-int}

Deletes several rows.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | The first row index to be deleted. |
| total_rows | int | Number of rows to be deleted. |
### Remarks

If the deleted range contains the top part(not whole) of the table(ListObject),
the ranged could not be deleted and nothing will be done.It works as MS Excel.

## delete_rows(row_index, total_rows, update_reference) {#int-int-bool}

Deletes multiple rows in the worksheet.

### Returns 





```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Row index. |
| total_rows | int | Number of rows to be deleted. |
| update_reference | bool | Indicates if update references in other worksheets. |



### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
