##PivotArea.PivotArea
PivotArea constructor. Presents the selected area of the PivotTable
## PivotArea constructor
Presents the selected area of the PivotTable.
```csharp
public PivotArea(PivotTable table)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | PivotTable |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaMethodctorWithPivotTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Demonstrate PivotArea constructor with PivotTable parameter
PivotArea pivotArea = new PivotArea(pivotTable);
// Configure pivot area
pivotArea.AxisType = PivotFieldType.Row;
pivotArea.RuleType = PivotAreaType.Normal;
// Save the workbook
workbook.Save("PivotAreaDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
