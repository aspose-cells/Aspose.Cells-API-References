##Enum DateTimeGroupingType
Aspose.Cells.DateTimeGroupingType enum. Specifies how to group dateTime values
## DateTimeGroupingType enumeration
Specifies how to group dateTime values.
```csharp
public enum DateTimeGroupingType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Day | `0` | Group by day. |
| Hour | `1` | Group by hour. |
| Minute | `2` | Group by Minute. |
| Month | `3` | Group by Month. |
| Second | `4` | Group by Second. |
| Year | `5` | Group by Year. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DateTimeGroupingTypeDemo
{
public static void DateTimeGroupingTypeExample()
{
// Creating a workbook and accessing the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding some sample data
worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));
// Creating an AutoFilter and setting the range
AutoFilter autoFilter = worksheet.AutoFilter;
autoFilter.Range = "A1:A6";
// Adding date filters with different DateTimeGroupingType
autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
// Saving the workbook
workbook.Save("DateTimeGroupingTypeExample.xlsx");
workbook.Save("DateTimeGroupingTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
