##PivotArea.IsRowGrandIncluded
PivotArea property. Indicates whether the row grand total is included
## PivotArea.IsRowGrandIncluded property
Indicates whether the row grand total is included.
```csharp
public bool IsRowGrandIncluded { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyIsRowGrandIncludedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Vegetable");
sheet.Cells["B1"].PutValue("Amount");
sheet.Cells["B2"].PutValue(50);
sheet.Cells["B3"].PutValue(30);
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create pivot format
int formatIndex = pivotTable.PivotFormats.Add();
PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
PivotArea pivotArea = pivotFormat.PivotArea;
// Demonstrate IsRowGrandIncluded property
pivotArea.AxisType = PivotFieldType.Data;
pivotArea.IsRowGrandIncluded = true;
pivotArea.IsColumnGrandIncluded = false;
// Apply style to highlight the grand row
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightGreen;
style.Pattern = BackgroundType.Solid;
pivotFormat.SetStyle(style);
workbook.Save("PivotAreaIsRowGrandIncludedDemo.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
