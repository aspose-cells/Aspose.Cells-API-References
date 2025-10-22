##PivotTable.FormatAll
PivotTable method. Format all the cell in the pivottable area
## PivotTable.FormatAll method
Format all the cell in the pivottable area
```csharp
public void FormatAll(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Style which is to format |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodFormatAllWithStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=Sheet1!A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Create and configure style
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 10;
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightGray;
style.Pattern = BackgroundType.Solid;
// Apply style to entire pivot table
pivotTable.FormatAll(style);
// Save the workbook
workbook.Save("PivotTableFormatAllDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
