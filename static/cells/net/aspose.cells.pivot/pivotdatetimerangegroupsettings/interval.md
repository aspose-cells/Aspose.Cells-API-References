##PivotDateTimeRangeGroupSettings.Interval
PivotDateTimeRangeGroupSettings property. Gets the internal of the group
## PivotDateTimeRangeGroupSettings.Interval property
Gets the internal of the group.
```csharp
public double Interval { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a worksheet with sample data
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Name = "Data";
// Add sample date data
dataSheet.Cells["A1"].PutValue("Date");
dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
dataSheet.Cells["A7"].PutValue(DateTime.Now);
// Add a pivot table worksheet
Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
// Add pivot table
int pivotIndex = pivotSheet.PivotTables.Add(
"=Data!A1:A7",
"A1",
"PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Add date field to row area
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
PivotField dateField = pivotTable.RowFields[0];
// Group by days with interval of 2
dateField.GroupBy(1, false);
PivotDateTimeRangeGroupSettings groupSettings =
(PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
// Since Interval is read-only, we need to set it during grouping
// The interval is actually set in the GroupBy method parameters
// Here we just verify the interval value
Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");
// Save the workbook
workbook.Save("PivotDateTimeGroupingDemo.xlsx");
}
}
}
```
### See Also
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
