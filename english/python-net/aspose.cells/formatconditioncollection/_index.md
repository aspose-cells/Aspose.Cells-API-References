---
title: FormatConditionCollection
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 700
url: /python-net/aspose.cells/formatconditioncollection/
---

## FormatConditionCollection class

Represents conditional formatting.<br/>             The FormatConditions can contain up to three conditional formats.

The FormatConditionCollection type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|count|Gets the count of the conditions.|
|range_count|Gets count of conditionally formatted ranges.|
## Indexer
| Name | Description |
| :- | :- |
|[index]|Gets the formatting condition by index.|
## Methods
| Name | Description |
| :- | :- |
|add_condition(type, operator_type, formula1, formula2)|Adds a formatting condition.|
|add_condition(type)|Adds a formatting condition.|
|remove_area(index)|Removes conditional formatted cell range by index.|
|remove_area(start_row, start_column, total_rows, total_columns)|Removes conditional formatted cell range by index.|
|add(cell_area, type, operator_type, formula1, formula2)|Adds a formatting condition and effected cell rang to the FormatConditions<br/>             The FormatConditions can contain up to three conditional formats.<br/>             References to the other sheets are not allowed in the formulas of conditional formatting.|
|add_area(cell_area)|Adds a conditional formatted cell range.|
|get_cell_area(index)|Gets the conditional formatted cell range by index.|
|remove_condition(index)|Removes the formatting condition by index.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

