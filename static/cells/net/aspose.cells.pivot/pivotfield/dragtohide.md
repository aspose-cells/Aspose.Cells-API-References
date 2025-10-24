##PivotField.DragToHide
PivotField property. Indicates whether the specified field can be dragged to the hide position. The default value is true
## PivotField.DragToHide property
Indicates whether the specified field can be dragged to the hide position. The default value is true.
```csharp
public bool DragToHide { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyDragToHideDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Category";
cells["A2"].Value = "Fruit";
cells["A3"].Value = "Vegetable";
cells["A4"].Value = "Fruit";
cells["A5"].Value = "Vegetable";
cells["B1"].Value = "Sales";
cells["B2"].Value = 100;
cells["B3"].Value = 150;
cells["B4"].Value = 200;
cells["B5"].Value = 250;
// Create pivot table - Get the index first, then get the PivotTable object
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and configure DragToHide
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pivotTable.RowFields[0];
rowField.DragToHide = true; // Core demonstration of the property
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldDragToHideDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
