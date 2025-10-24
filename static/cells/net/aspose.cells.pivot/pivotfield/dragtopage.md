##PivotField.DragToPage
PivotField property. Indicates whether the specified field can be dragged to the page position. The default value is true
## PivotField.DragToPage property
Indicates whether the specified field can be dragged to the page position. The default value is true.
```csharp
public bool DragToPage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyDragToPageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Product";
cells["A2"].Value = "Bikes";
cells["A3"].Value = "Cars";
cells["A4"].Value = "Bikes";
cells["A5"].Value = "Cars";
cells["B1"].Value = "Region";
cells["B2"].Value = "North";
cells["B3"].Value = "South";
cells["B4"].Value = "North";
cells["B5"].Value = "South";
cells["C1"].Value = "Sales";
cells["C2"].Value = 1000;
cells["C3"].Value = 2000;
cells["C4"].Value = 3000;
cells["C5"].Value = 4000;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields and configure DragToPage
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
PivotField regionField = pivotTable.PageFields[fieldIndex];
// Demonstrate DragToPage property
regionField.DragToPage = false; // Disable dragging to page area
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save workbook
workbook.Save("PivotFieldDragToPageDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
