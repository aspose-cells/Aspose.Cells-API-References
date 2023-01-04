---
title: set_manual_group_field method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 210
url: /python-net/aspose.cells.pivot/pivottable/set_manual_group_field/
is_root: false
---

## set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-float-float-list-float}

Sets manual field group by the PivotTable.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| base_field_index | int | The row or column field index in the base fields |
| start_val | float | Specifies the starting value for numeric grouping. |
| end_val | float | Specifies the ending value for numeric grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | float | Specifies the interval number group by  numeric grouping. |


## set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-float-float-list-float}

Sets manual field group by the PivotTable.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| pivot_field | [PivotField](/cells/python-net/aspose.cells.pivot/pivotfield) | The row or column field in the base fields |
| start_val | float | Specifies the starting value for numeric grouping. |
| end_val | float | Specifies the ending value for numeric grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | float | Specifies the interval number group by numeric grouping. |


## set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num) {#int-DateTime-DateTime-list-int}

Sets manual field group by the PivotTable.



```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| base_field_index | int | The row or column field index in the base fields |
| start_val | DateTime | Specifies the starting value for date grouping. |
| end_val | DateTime | Specifies the ending value for date grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |


## set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num) {#PivotField-DateTime-DateTime-list-int}

Sets manual field group by the PivotTable.



```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| pivot_field | [PivotField](/cells/python-net/aspose.cells.pivot/pivotfield) | The row or column field in the base fields |
| start_val | DateTime | Specifies the starting value for date grouping. |
| end_val | DateTime | Specifies the ending value for date grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |



### See Also
* module [aspose.cells.pivot](../../)
* class [PivotTable](/cells/python-net/aspose.cells.pivot/pivottable)
