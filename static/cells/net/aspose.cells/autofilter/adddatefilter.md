##AutoFilter.AddDateFilter
AutoFilter method. Adds a date filter
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
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodAddDateFilterWithInt32DateTimeGroupingTypeInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
AutoFilter autoFilter = worksheet.AutoFilter;
autoFilter.Range = "A1:A5";
autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
autoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2023, 1, 2, 0, 0, 0);
workbook.Save("AutoFilterAddDateFilterExample.xlsx");
}
}
}
```
### See Also
* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
