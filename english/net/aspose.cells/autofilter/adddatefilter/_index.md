---
title: AutoFilter.AddDateFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds a date filter
type: docs
url: /net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Adds a date filter.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | DateTimeGroupingType | The grouping type |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |
| hour | Int32 | The hour. |
| minute | Int32 | The minute. |
| second | Int32 | The second. |

### Remarks

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


