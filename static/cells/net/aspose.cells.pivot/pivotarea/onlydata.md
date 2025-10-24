##PivotArea.OnlyData
PivotArea property. Indicates whether only the data values in the data area of the view for an item selection are selected and does not include the item labels
## PivotArea.OnlyData property
Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.
```csharp
public bool OnlyData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyOnlyDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Electronics");
worksheet.Cells["A3"].PutValue("Clothing");
worksheet.Cells["A4"].PutValue("Food");
worksheet.Cells["B1"].PutValue("Revenue");
worksheet.Cells["B2"].PutValue(5000);
worksheet.Cells["B3"].PutValue(3000);
worksheet.Cells["B4"].PutValue(2000);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Configure pivot area
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.RuleType = PivotAreaType.Normal;
pivotArea.OnlyData = true; // Key property demonstration
pivotArea.IsRowGrandIncluded = false;
// Output configuration
Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
workbook.Save("PivotAreaOnlyDataDemo.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
