---
title: SeriesCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 240
url: /python-net/aspose.cells.charts/seriescollection/
is_root: false
---

## SeriesCollection class

Encapsulates a collection of [Series](/cells/python-net/aspose.cells.charts/series) objects.



The SeriesCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [category_data](/cells/python-net/aspose.cells.charts/seriescollection/category_data) | Gets or sets the range of category Axis values. <br/>It can be a range of cells (such as, "d1:e10"), <br/>or a sequence of values (such as,"{2,6,8,10}"). |
| [second_category_data](/cells/python-net/aspose.cells.charts/seriescollection/second_category_data) | Gets or sets the range of second category Axis values. <br/>It can be a range of cells (such as, "d1:e10"), <br/>or a sequence of values (such as,"{2,6,8,10}"). <br/>Only effects when some ASerieses plot on the second axis. |
| [is_color_varied](/cells/python-net/aspose.cells.charts/seriescollection/is_color_varied) | Represents if the color of points is varied. |
| [capacity](/cells/python-net/aspose.cells.charts/seriescollection/capacity) | Gets or sets the number of elements that the array list can contain. |


### Methods
| Method | Description |
| :- | :- |
| [add(area, is_vertical)](/cells/python-net/aspose.cells.charts/seriescollection/add/#str-bool) | Adds the [SeriesCollection](/cells/python-net/aspose.cells.charts/seriescollection) collection to a chart. |
| [add(area, is_vertical, check_labels)](/cells/python-net/aspose.cells.charts/seriescollection/add/#str-bool-bool) | Adds the [SeriesCollection](/cells/python-net/aspose.cells.charts/seriescollection) collection to a chart. |
| [copy_to(array)](/cells/python-net/aspose.cells.charts/seriescollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [copy_to(index, array, array_index, count)](/cells/python-net/aspose.cells.charts/seriescollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [index_of(item, index)](/cells/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [index_of(item, index, count)](/cells/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [last_index_of(item)](/cells/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [last_index_of(item, index)](/cells/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [last_index_of(item, index, count)](/cells/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [get_series_by_order(order)](/cells/python-net/aspose.cells.charts/seriescollection/get_series_by_order/#int) | Gets the [Series](/cells/python-net/aspose.cells.charts/series) element by order. |
| [change_series_order(source_index, dest_index)](/cells/python-net/aspose.cells.charts/seriescollection/change_series_order/#int-int) | Directly changes the orders of the two series. |
| [set_series_names(start_index, area, is_vertical)](/cells/python-net/aspose.cells.charts/seriescollection/set_series_names/#int-str-bool) | Sets the name of all the serieses in the chart. |
| [add_r1c1(area, is_vertical)](/cells/python-net/aspose.cells.charts/seriescollection/add_r1c1/#str-bool) | Adds the [SeriesCollection](/cells/python-net/aspose.cells.charts/seriescollection) collection to a chart. |
| [binary_search(item)](/cells/python-net/aspose.cells.charts/seriescollection/binary_search/#Series) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |


### See Also

* module [aspose.cells.charts](../)
