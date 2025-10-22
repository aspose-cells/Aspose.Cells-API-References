##WorkbookSettings.UpdateAdjacentCellsBorder
WorkbookSettings property. Indicates whether update adjacent cells border
## WorkbookSettings.UpdateAdjacentCellsBorder property
Indicates whether update adjacent cells' border.
```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```
### Remarks
The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Enable updating adjacent cells' borders
workbook.Settings.UpdateAdjacentCellsBorder = true;
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set value and apply border to cell A1
worksheet.Cells["A1"].PutValue("Sample");
Style styleA1 = workbook.CreateStyle();
styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
worksheet.Cells["A1"].SetStyle(styleA1);
// Set value to adjacent cell B1 (right of A1)
worksheet.Cells["B1"].PutValue("Adjacent");
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
