##PivotArea.IsColumnGrandIncluded
PivotArea property. Indicates whether the column grand total is included
## PivotArea.IsColumnGrandIncluded property
Indicates whether the column grand total is included.
```csharp
public bool IsColumnGrandIncluded { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyIsColumnGrandIncludedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Fruit";
worksheet.Cells["A3"].Value = "Vegetable";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 150;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Configure pivot area
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
pivotArea.IsRowGrandIncluded = true;
pivotArea.RuleType = PivotAreaType.Normal;
// Save the workbook
workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
