##PivotField.DragToData
PivotField property. Indicates whether the specified field can be dragged to the data position. The default value is true
## PivotField.DragToData property
Indicates whether the specified field can be dragged to the data position. The default value is true.
```csharp
public bool DragToData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyDragToDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Product";
cells["B1"].Value = "Quarter";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Bikes";
cells["A3"].Value = "Bikes";
cells["A4"].Value = "Cars";
cells["A5"].Value = "Cars";
cells["B2"].Value = "Q1";
cells["B3"].Value = "Q2";
cells["B4"].Value = "Q1";
cells["B5"].Value = "Q2";
cells["C2"].Value = 1000;
cells["C3"].Value = 1500;
cells["C4"].Value = 2000;
cells["C5"].Value = 2500;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and configure DragToData
int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
PivotField rowField = pivotTable.RowFields[rowFieldIndex];
rowField.DragToData = true; // Allow dragging this field to data area
// Add column field
pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldDragToDataDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
