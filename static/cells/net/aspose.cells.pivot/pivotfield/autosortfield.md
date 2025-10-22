##PivotField.AutoSortField
PivotField property. Represents the index of field which is auto sorted. 1 means PivotField itselfothers means the position of the data fields
## PivotField.AutoSortField property
Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.
```csharp
public int AutoSortField { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyAutoSortFieldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Branch";
cells["B1"].Value = "Sales";
cells["A2"].Value = "North";
cells["B2"].Value = 1000;
cells["A3"].Value = "South";
cells["B3"].Value = 1500;
cells["A4"].Value = "East";
cells["B4"].Value = 800;
cells["A5"].Value = "West";
cells["B5"].Value = 1200;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields["Branch"];
// Configure auto sort
pivotField.IsAutoSort = true;
pivotField.IsAscendSort = true;
pivotField.AutoSortField = 0; // Sort by first data field (Sales)
// Calculate data and refresh
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldAutoSortDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
