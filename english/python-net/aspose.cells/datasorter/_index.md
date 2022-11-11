---
title: DataSorter
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 420
url: /python-net/aspose.cells/datasorter/
---

## DataSorter class

Summary description for DataSorter.

The DataSorter type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|keys|Gets the key list of data sorter.|
|has_headers|Represents whether the range has headers.|
|key1|Represents first sorted column index(absolute position, column A is 0, B is 1, ...).|
|order1|Represents sort order of the first key.|
|key2|Represents second sorted column index(absolute position, column A is 0, B is 1, ...).|
|order2|Represents sort order of the second key.|
|key3|Represents third sorted column index(absolute position, column A is 0, B is 1, ...).|
|order3|Represents sort order of the third key.|
|sort_left_to_right|True means that sorting orientation is from left to right.<br/>            False means that sorting orientation is from top to bottom.<br/>            The default value is false.|
|case_sensitive|Gets and sets whether case sensitive when comparing string.|
|sort_as_number|Indicates whether sorting anything that looks like a number.|
## Methods
| Name | Description |
| :- | :- |
|add_key(key, order)|Adds sorted column index and sort order.|
|add_key(key, order, custom_list)|Adds sorted column index and sort order with custom sort list.|
|add_key(key, type, order, custom_list)|Adds sorted column index and sort order with custom sort list.|
|add_key(key, order, custom_list)|Adds sorted column index and sort order with custom sort list.|
|sort(cells, start_row, start_column, end_row, end_column)|Sorts the data of the area.|
|sort(cells, area)|Sort the data of the area.|
|sort()|Sorts the data of the area.|
|clear()|Clear all settings.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

