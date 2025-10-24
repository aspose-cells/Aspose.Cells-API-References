##WorkbookSettings.HidePivotFieldList
WorkbookSettings property. Gets and sets whether hide the field list for the PivotTable
## WorkbookSettings.HidePivotFieldList property
Gets and sets whether hide the field list for the PivotTable.
```csharp
public bool HidePivotFieldList { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyHidePivotFieldListDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B3"].PutValue(200);
sheet.Cells["A4"].PutValue("A");
sheet.Cells["B4"].PutValue(150);
// Create pivot table
int index = workbook.Worksheets.Add(SheetType.Worksheet);
Worksheet pivotSheet = workbook.Worksheets[index];
pivotSheet.Name = "PivotTable";
int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Access workbook settings and set HidePivotFieldList property
WorkbookSettings settings = workbook.Settings;
settings.HidePivotFieldList = true; // Hide the pivot field list
// Save the workbook
workbook.Save("HidePivotFieldListDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
