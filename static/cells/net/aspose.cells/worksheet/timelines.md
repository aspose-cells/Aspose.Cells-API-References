##Worksheet.Timelines
Worksheet property. Get the Timeline collection in the worksheet
## Worksheet.Timelines property
Get the Timeline collection in the worksheet
```csharp
public TimelineCollection Timelines { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTimelinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Ship Date";
sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 1000;
sheet.Cells["B3"].Value = 2000;
sheet.Cells["B4"].Value = 3000;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add timeline control for the pivot table
sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");
// Save the workbook
workbook.Save("TimelineDemo.xlsx");
}
}
}
```
### See Also
* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
