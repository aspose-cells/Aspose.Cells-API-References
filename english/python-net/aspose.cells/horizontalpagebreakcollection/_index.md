---
title: HorizontalPageBreakCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 760
url: /python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---

## HorizontalPageBreakCollection class

Encapsulates a collection of [HorizontalPageBreak](/cells/python-net/aspose.cells/horizontalpagebreak) objects.



The HorizontalPageBreakCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Gets or sets the number of elements that the array list can contain. |


### Methods
| Method | Description |
| :- | :- |
| [add(row, start_column, end_column)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Adds a horizontal page break to the collection. |
| [add(row)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Adds a horizontal page break to the collection. |
| [add(row, column)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Adds a horizontal page break to the collection. |
| [add(cell_name)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Adds a horizontal page break to the collection. |
| [copy_to(array)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [copy_to(index, array, array_index, count)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [index_of(item, index)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [index_of(item, index, count)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [last_index_of(item)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [last_index_of(item, index)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [last_index_of(item, index, count)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [binary_search(item)](/cells/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |



### Example 


```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

### See Also
* module [aspose.cells](..)
* class [HorizontalPageBreak](/cells/python-net/aspose.cells/horizontalpagebreak)
