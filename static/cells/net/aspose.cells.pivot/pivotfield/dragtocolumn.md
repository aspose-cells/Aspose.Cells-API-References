##PivotField.DragToColumn
PivotField property. Indicates whether the specified field can be dragged to the column position. The default value is true
## PivotField.DragToColumn property
Indicates whether the specified field can be dragged to the column position. The default value is true.
```csharp
public bool DragToColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyDragToColumnDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Fruit");
worksheet.Cells["A4"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Item");
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["B3"].PutValue("Orange");
worksheet.Cells["B4"].PutValue("Carrot");
worksheet.Cells["C1"].PutValue("Quantity");
worksheet.Cells["C2"].PutValue(10);
worksheet.Cells["C3"].PutValue(15);
worksheet.Cells["C4"].PutValue(8);
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the data field and set DragToColumn to true
PivotField quantityField = pivotTable.DataFields[0];
quantityField.DragToColumn = true; // This allows the field to be dragged to column area
quantityField.DisplayName = "Total Quantity";
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
