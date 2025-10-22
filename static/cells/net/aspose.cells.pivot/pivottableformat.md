##Class PivotTableFormat
Aspose.Cells.Pivot.PivotTableFormat class. Represents the format defined in the PivotTable
## PivotTableFormat class
Represents the format defined in the PivotTable.
```csharp
public class PivotTableFormat
```
## Properties
| Name | Description |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Gets the pivot area. |
## Methods
| Name | Description |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Gets the formatted style. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Sets the style of the pivot area. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
namespace AsposeCellsExamples
{
public class PivotTableFormatDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Vegetable");
sheet.Cells["B1"].PutValue("Amount");
sheet.Cells["B2"].PutValue(50);
sheet.Cells["B3"].PutValue(30);
// Add a pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount
// Access the PivotTableFormatCollection
PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;
// Add a new format to the collection
int formatIndex = pivotFormats.Add();
PivotTableFormat pivotFormat = pivotFormats[formatIndex];
// Access the PivotArea of the format
PivotArea pivotArea = pivotFormat.PivotArea;
pivotArea.AxisType = PivotFieldType.Data;
pivotArea.IsRowGrandIncluded = true;
pivotArea.IsColumnGrandIncluded = true;
// Create a new style
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
// Apply the style to the PivotTableFormat
pivotFormat.SetStyle(style);
// Save the workbook
workbook.Save("PivotTableFormatDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
