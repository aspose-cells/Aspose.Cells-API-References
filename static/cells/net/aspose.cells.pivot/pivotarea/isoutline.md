##PivotArea.IsOutline
PivotArea property. Indicates whether the rule refers to an area that is in outline mode
## PivotArea.IsOutline property
Indicates whether the rule refers to an area that is in outline mode.
```csharp
public bool IsOutline { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyIsOutlineDemo
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
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
// Create and configure PivotArea
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.IsOutline = false; // Disable outline style
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);
// Save the workbook
workbook.Save("PivotAreaIsOutlineDemo.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
