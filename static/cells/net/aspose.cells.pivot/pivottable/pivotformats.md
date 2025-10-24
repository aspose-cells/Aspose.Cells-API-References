##PivotTable.PivotFormats
PivotTable property. Gets the collection of formats applied to PivotTable
## PivotTable.PivotFormats property
Gets the collection of formats applied to PivotTable.
```csharp
public PivotTableFormatCollection PivotFormats { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPivotFormatsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["B1"].Value = "Quantity";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["B2"].Value = 10;
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["B3"].Value = 15;
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["B4"].Value = 20;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Create style for formatting
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.LightBlue;
style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.Black);
style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.Black);
style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.Black);
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
// Apply formatting to pivot table data area
pivotTable.PivotFormats.FormatArea(
PivotFieldType.Data,
0,
PivotFieldSubtotalType.None,
PivotTableSelectionType.DataAndLabel,
false,
false,
style);
// Save the workbook
workbook.Save("PivotTableWithFormats.xlsx");
}
}
}
```
### See Also
* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
