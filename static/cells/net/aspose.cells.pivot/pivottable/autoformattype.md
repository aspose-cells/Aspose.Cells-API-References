##PivotTable.AutoFormatType
PivotTable property. Gets and sets the auto format type of PivotTable
## PivotTable.AutoFormatType property
Gets and sets the auto format type of PivotTable.
```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyAutoFormatTypeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Product");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Electronics");
worksheet.Cells["B2"].PutValue("Laptop");
worksheet.Cells["C2"].PutValue(1200);
worksheet.Cells["A3"].PutValue("Electronics");
worksheet.Cells["B3"].PutValue("Phone");
worksheet.Cells["C3"].PutValue(800);
worksheet.Cells["A4"].PutValue("Furniture");
worksheet.Cells["B4"].PutValue("Chair");
worksheet.Cells["C4"].PutValue(150);
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
// Demonstrate AutoFormatType property
pivotTable.IsAutoFormat = true;
pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
// Save the workbook
workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
