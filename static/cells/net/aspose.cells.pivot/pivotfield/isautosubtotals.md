##PivotField.IsAutoSubtotals
PivotField property. Indicates whether the specified field shows automatic subtotals. Default is true
## PivotField.IsAutoSubtotals property
Indicates whether the specified field shows automatic subtotals. Default is true.
```csharp
public bool IsAutoSubtotals { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyIsAutoSubtotalsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Bikes";
worksheet.Cells["A3"].Value = "Bikes";
worksheet.Cells["A4"].Value = "Cars";
worksheet.Cells["A5"].Value = "Cars";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
worksheet.Cells["B5"].Value = 4000;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add field to row area and set IsAutoSubtotals to false
int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
PivotField rowField = pivotTable.RowFields[fieldIndex];
rowField.IsAutoSubtotals = false; // Disable automatic subtotals
// Add field to data area
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
