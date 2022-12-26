---
title: DataSorter class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 420
url: /python-net/aspose.cells/datasorter/
is_root: false
---

## DataSorter class

Summary description for DataSorter.



The DataSorter type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [keys](/cells/python-net/aspose.cells/datasorter/keys) | Gets the key list of data sorter. |
| [has_headers](/cells/python-net/aspose.cells/datasorter/has_headers) | Represents whether the range has headers. |
| [key1](/cells/python-net/aspose.cells/datasorter/key1) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order1](/cells/python-net/aspose.cells/datasorter/order1) | Represents sort order of the first key. |
| [key2](/cells/python-net/aspose.cells/datasorter/key2) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order2](/cells/python-net/aspose.cells/datasorter/order2) | Represents sort order of the second key. |
| [key3](/cells/python-net/aspose.cells/datasorter/key3) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order3](/cells/python-net/aspose.cells/datasorter/order3) | Represents sort order of the third key. |
| [sort_left_to_right](/cells/python-net/aspose.cells/datasorter/sort_left_to_right) | True means that sorting orientation is from left to right.<br/>False means that sorting orientation is from top to bottom.<br/>The default value is false. |
| [case_sensitive](/cells/python-net/aspose.cells/datasorter/case_sensitive) | Gets and sets whether case sensitive when comparing string. |
| [sort_as_number](/cells/python-net/aspose.cells/datasorter/sort_as_number) | Indicates whether sorting anything that looks like a number. |


### Methods
| Method | Description |
| :- | :- |
| [add_key(key, order)](/cells/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Adds sorted column index and sort order. |
| [add_key(key, order, custom_list)](/cells/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Adds sorted column index and sort order with custom sort list. |
| [add_key(key, type, order, custom_list)](/cells/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Adds sorted column index and sort order with custom sort list. |
| [add_key(key, order, custom_list)](/cells/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) |  |
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Sorts the data of the area. |
| [sort(cells, area)](/cells/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Sort the data of the area. |
| [sort()](/cells/python-net/aspose.cells/datasorter/sort/#) | Sort the data in the range. |
| [clear()](/cells/python-net/aspose.cells/datasorter/clear/#) | Clear all settings. |


### See Also

* module [aspose.cells](../)
