##set_manual_group_field method
## set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num) {#int-float-float-list-float}
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
### Remarks
NOTE: This method is now obsolete. Instead,
please use PivotField.GroupBy() method.
This method will be removed 12 months later since October 2023.
Aspose apologizes for any inconvenience you may have experienced.
## set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num) {#aspose.cells.pivot.PivotField-float-float-list-float}
Sets manual field group by the PivotTable.
```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot_field | aspose.cells.pivot.PivotField | The row or column field in the base fields |
| start_val | float | Specifies the starting value for numeric grouping. |
| end_val | float | Specifies the ending value for numeric grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | float | Specifies the interval number group by numeric grouping. |
### Remarks
NOTE: This method is now obsolete. Instead,
please use PivotField.GroupBy() method.
This method will be removed 12 months later since October 2023.
Aspose apologizes for any inconvenience you may have experienced.
## set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num) {#int-System.DateTime-System.DateTime-list-int}
Sets manual field group by the PivotTable.
```python
def set_manual_group_field(self, base_field_index, start_val, end_val, group_by_list, interval_num):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| base_field_index | int | The row or column field index in the base fields |
| start_val | System.DateTime | Specifies the starting value for date grouping. |
| end_val | System.DateTime | Specifies the ending value for date grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |
### Remarks
NOTE: This method is now obsolete. Instead,
please use PivotField.GroupBy() method.
This method will be removed 12 months later since October 2023.
Aspose apologizes for any inconvenience you may have experienced.
## set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num) {#aspose.cells.pivot.PivotField-System.DateTime-System.DateTime-list-int}
Sets manual field group by the PivotTable.
```python
def set_manual_group_field(self, pivot_field, start_val, end_val, group_by_list, interval_num):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot_field | aspose.cells.pivot.PivotField | The row or column field in the base fields |
| start_val | System.DateTime | Specifies the starting value for date grouping. |
| end_val | System.DateTime | Specifies the ending value for date grouping. |
| group_by_list | list | Specifies the grouping type list. Specified by PivotTableGroupType |
| interval_num | int | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |
### Remarks
NOTE: This method is now obsolete. Instead,
please use PivotField.GroupBy() method.
This method will be removed 12 months later since October 2023.
Aspose apologizes for any inconvenience you may have experienced.
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotTable`](/cells/python-net/aspose.cells.pivot/pivottable)
