##PivotDateTimeRangeGroupSettings.Start
PivotDateTimeRangeGroupSettings property. Gets the start date time of the group
## PivotDateTimeRangeGroupSettings.Start property
Gets the start date time of the group.
```csharp
public DateTime Start { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotDateTimeRangeGroupSettingsPropertyStartDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Group by date range
PivotField dateField = pivotTable.RowFields[0];
DateTime startDate = new DateTime(2023, 1, 1);
DateTime endDate = new DateTime(2023, 12, 31);
dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);
// Access group settings and demonstrate Start property
PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
Console.WriteLine("Group Start Date: " + groupSettings.Start);
// Save workbook
workbook.Save("PivotDateTimeRangeGroupSettingsStartDemo.xlsx");
}
}
}
```
### See Also
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
