##PivotField.IsAscendSort
PivotField property. Indicates whether the specified PivotTable field is autosorted ascending
## PivotField.IsAscendSort property
Indicates whether the specified PivotTable field is autosorted ascending.
```csharp
public bool IsAscendSort { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyIsAscendSortDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Product";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["A2"].Value = "B";
sheet.Cells["A3"].Value = "C";
sheet.Cells["A4"].Value = "A";
sheet.Cells["B2"].Value = 150;
sheet.Cells["B3"].Value = 300;
sheet.Cells["B4"].Value = 200;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Configure sorting
PivotField sortField = pivotTable.RowFields[0];
sortField.IsAutoSort = true;
sortField.IsAscendSort = false; // Demonstrate descending sort
sortField.AutoSortField = 0; // Sort by first data field
// Refresh and calculate pivot table
pivotTable.RefreshDataFlag = true;
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldIsAscendSortDemo_out.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
