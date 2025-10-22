##add_date_filter method
## add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second) {#int-aspose.cells.DateTimeGroupingType-int-int-int-int-int-int}
Adds a date filter.
```python
def add_date_filter(self, field_index, date_time_grouping_type, year, month, day, hour, minute, second):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter
| date_time_grouping_type | aspose.cells.DateTimeGroupingType | The grouping type |
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
* module [`aspose.cells`](../../)
* class [`AutoFilter`](/cells/python-net/aspose.cells/autofilter)
