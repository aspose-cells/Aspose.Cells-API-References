---
title: custom method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 70
url: /python-net/aspose.cells/autofilter/custom/
is_root: false
---

## custom(field_index, operator_type1, criteria1) {#int-FilterOperatorType-any}

Filters a list with a custom criteria.



```python
def custom(self, field_index, operator_type1, criteria1):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| operator_type1 | [FilterOperatorType](/cells/python-net/aspose.cells/filteroperatortype) | The filter operator type |
| criteria1 | any | The custom criteria |


## custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2) {#int-FilterOperatorType-any-bool-FilterOperatorType-any}

Filters a list with custom criteria.



```python
def custom(self, field_index, operator_type1, criteria1, is_and, operator_type2, criteria2):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| operator_type1 | [FilterOperatorType](/cells/python-net/aspose.cells/filteroperatortype) | The filter operator type |
| criteria1 | any | The custom criteria |
| is_and | bool |  |
| operator_type2 | [FilterOperatorType](/cells/python-net/aspose.cells/filteroperatortype) | The filter operator type |
| criteria2 | any | The custom criteria |



### See Also
* module [aspose.cells](../../)
* class [AutoFilter](/cells/python-net/aspose.cells/autofilter)
