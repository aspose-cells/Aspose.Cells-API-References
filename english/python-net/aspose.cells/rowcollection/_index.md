---
title: RowCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1310
url: /python-net/aspose.cells/rowcollection/
is_root: false
---

## RowCollection class

Collects the [Row](/cells/python-net/aspose.cells/row) objects that represent the individual rows in a worksheet.



The RowCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [count](/cells/python-net/aspose.cells/rowcollection/count) | Gets the number of rows in this collection. |



Gets a [Row](/cells/python-net/aspose.cells/row) object by given row index. The Row object of given row index will be instantiated if it does not exist before.
### Indexer
| Name | Description |
| :- | :- |
| [index] |  |


### Methods
| Method | Description |
| :- | :- |
| [get_row_by_index(index)](/cells/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Gets the row object by the position in the list. |
| [clear()](/cells/python-net/aspose.cells/rowcollection/clear/#) | Clear all rows and cells. |
| [remove_at(index)](/cells/python-net/aspose.cells/rowcollection/remove_at/#int) | Remove the row at the specified index |



### Example 


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

### See Also
* module [aspose.cells](..)
* class [Row](/cells/python-net/aspose.cells/row)
