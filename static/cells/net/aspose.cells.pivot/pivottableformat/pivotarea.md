##PivotTableFormat.PivotArea
PivotTableFormat property. Gets the pivot area
## PivotTableFormat.PivotArea property
Gets the pivot area.
```csharp
public PivotArea PivotArea { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableFormatPropertyPivotAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Vegetable");
sheet.Cells["B1"].PutValue("Amount");
sheet.Cells["B2"].PutValue(50);
sheet.Cells["B3"].PutValue(30);
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields to pivot areas
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get pivot format and configure its pivot area
int formatIndex = pivotTable.PivotFormats.Add();
PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
PivotArea pivotArea = pivotFormat.PivotArea;
// Set pivot area properties
pivotArea.AxisType = PivotFieldType.Data;
pivotArea.IsRowGrandIncluded = true;
pivotArea.IsColumnGrandIncluded = true;
// Create and apply style to the pivot area
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
pivotFormat.SetStyle(style);
// Save the workbook
workbook.Save("PivotTableWithPivotArea.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../../pivotarea/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
