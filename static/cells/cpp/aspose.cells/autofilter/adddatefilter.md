##Aspose::Cells::AutoFilter::AddDateFilter method
'Aspose::Cells::AutoFilter::AddDateFilter method. Adds a date filter in C++.'
## AutoFilter::AddDateFilter method
Adds a date filter.
```cpp
void Aspose::Cells::AutoFilter::AddDateFilter(int32_t fieldIndex, DateTimeGroupingType dateTimeGroupingType, int32_t year, int32_t month, int32_t day, int32_t hour, int32_t minute, int32_t second)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int32_t | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | DateTimeGroupingType | The grouping type |
| year | int32_t | The year. |
| month | int32_t | The month. |
| day | int32_t | The day. |
| hour | int32_t | The hour. |
| minute | int32_t | The minute. |
| second | int32_t | The second. |
## Remarks
If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.
## See Also
* Enum [DateTimeGroupingType](../../datetimegroupingtype/)
* Class [AutoFilter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
