##Enum PivotGroupByType
Aspose.Cells.Pivot.PivotGroupByType enum. Represents group by type
## PivotGroupByType enumeration
Represents group by type.
```csharp
public enum PivotGroupByType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| RangeOfValues | `0` | Group by numbers. |
| Numbers | `0` | Group by numbers. |
| Seconds | `1` | Presents Seconds groupby type. |
| Minutes | `2` | Presents Minutes groupby type. |
| Hours | `3` | Presents Hours groupby type. |
| Days | `4` | Presents Days groupby type. |
| Months | `5` | Presents Months groupby type. |
| Quarters | `6` | Presents Quarters groupby type. |
| Years | `7` | Presents Years groupby type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotGroupByTypeDemo
{
public static void PivotGroupByTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Date");
Style style = workbook.CreateStyle();
style.Number = 14;//m/d/yyy
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A2"].SetStyle(style);
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A3"].SetStyle(style);
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["A4"].SetStyle(style);
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field
//TODO
PivotField dateField = pivotTable.RowFields[0];
DateTime start = new DateTime(2023, 1, 1);
DateTime end = new DateTime(2023, 12, 31);
dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);
// Access the group settings
PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
// Output the group settings
Console.WriteLine("Group Type: " + groupSettings.Type);
Console.WriteLine("Start Date: " + groupSettings.Start);
Console.WriteLine("End Date: " + groupSettings.End);
Console.WriteLine("Interval: " + groupSettings.Interval);
Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));
// Save the workbook
workbook.Save("PivotGroupByTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
