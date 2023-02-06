---
title: add_date_filter method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/autofilter/add_date_filter/
is_root: false
---

## add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-DateTimeGroupingType-int-int-int-int-int-int}

Adds a date filter.



```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| date_time_grouping_type | [DateTimeGroupingType](/cells/python-net/aspose.cells/datetimegroupingtype) | [DateTimeGroupingType](/cells/python-net/aspose.cells/datetimegroupingtype) |
| year | int | The year. |
| month | int | The month. |
| day | int | The day. |
| hour | int | The hour. |
| minute | int | The minute. |
| second | int | The second. |
### Remarks

If DateTimeGroupingType is Year, only the param year effects.
If DateTiemGroupingType is Month, only the param year and month effect.


### See Also
* module [aspose.cells](../../)
* class [AutoFilter](/cells/python-net/aspose.cells/autofilter)
* class [DateTimeGroupingType](/cells/python-net/aspose.cells/datetimegroupingtype)
