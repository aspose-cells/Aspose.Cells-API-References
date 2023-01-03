---
title: subtotal method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 920
url: /python-net/aspose.cells/cells/subtotal/
is_root: false
---

## subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}

Creates subtotals for the range.



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ca | [CellArea](/cells/python-net/aspose.cells/cellarea) | The range |
| group_by | int | The field to group by, as a zero-based integer offset |
| function | [ConsolidationFunction](/cells/python-net/aspose.cells/consolidationfunction) | The subtotal function. |
| total_list | list | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |


## subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}

Creates subtotals for the range.



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ca | [CellArea](/cells/python-net/aspose.cells/cellarea) | The range |
| group_by | int | The field to group by, as a zero-based integer offset |
| function | [ConsolidationFunction](/cells/python-net/aspose.cells/consolidationfunction) | The subtotal function. |
| total_list | list | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | bool | Indicates whether replace the current subtotals |
| page_breaks | bool | Indicates whether add page break between groups |
| summary_below_data | bool | Indicates whether add summary below data. |



### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
