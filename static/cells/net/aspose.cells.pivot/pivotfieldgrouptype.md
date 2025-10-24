##Enum PivotFieldGroupType
Aspose.Cells.Pivot.PivotFieldGroupType enum. Represents the group type of pivot field
## PivotFieldGroupType enumeration
Represents the group type of pivot field.
```csharp
public enum PivotFieldGroupType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No group |
| DateTimeRange | `1` | Grouped by DateTime range. |
| NumbericRange | `2` | Grouped by numberic range. |
| Discrete | `3` | Grouped by discrete points. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotClassPivotFieldGroupTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Date");
Style style = workbook.CreateStyle();
style.Number = 14; // m/d/yyyy format
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
// Group the date field
PivotField dateField = pivotTable.RowFields[0];
DateTime start = new DateTime(2023, 1, 1);
DateTime end = new DateTime(2023, 12, 31);
dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);
// Access and display group settings
PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
Console.WriteLine("Group Type: " + groupSettings.Type);
Console.WriteLine("Interval: " + groupSettings.Interval);
Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));
// Save the workbook
workbook.Save("PivotFieldGroupTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
