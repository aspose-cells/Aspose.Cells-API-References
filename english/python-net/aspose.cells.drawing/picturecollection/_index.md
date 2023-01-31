---
title: PictureCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 460
url: /python-net/aspose.cells.drawing/picturecollection/
is_root: false
---

## PictureCollection class

Encapsulates a collection of [Picture](/cells/python-net/aspose.cells.drawing/picture) objects.



The PictureCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.drawing/picturecollection/capacity) | Gets or sets the number of elements that the array list can contain. |


### Methods
| Method | Description |
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Adds a picture to the collection. |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Adds a picture to the collection. |
| [add(upper_left_row, upper_left_column, stream)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Adds a picture to the collection. |
| [add(upper_left_row, upper_left_column, file_name)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Adds a picture to the collection. |
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Adds a picture to the collection. |
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Adds a picture to the collection. |
| [copy_to(array)](/cells/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [copy_to(index, array, array_index, count)](/cells/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [index_of(item, index)](/cells/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [index_of(item, index, count)](/cells/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [last_index_of(item)](/cells/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [last_index_of(item, index)](/cells/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [last_index_of(item, index, count)](/cells/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [binary_search(item)](/cells/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |


### Example 


```
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()

# get PictureCollection
pictures = workbook.worksheets[0].pictures

# do your business
# Save the excel file.
workbook.save("result.xlsx")

```
### See Also

* module [aspose.cells.drawing](../)
