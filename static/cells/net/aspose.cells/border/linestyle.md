##Border.LineStyle
Border property. Gets or sets the cell border type
## Border.LineStyle property
Gets or sets the cell border type.
```csharp
public CellBorderType LineStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BorderPropertyLineStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell and get its style
Cell cell = worksheet.Cells["B2"];
Style style = cell.GetStyle();
// Set different border line styles
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BorderLineStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
