##BorderCollection.DiagonalStyle
BorderCollection property. Gets or sets the style of Diagonal lines
## BorderCollection.DiagonalStyle property
Gets or sets the style of Diagonal lines.
```csharp
public CellBorderType DiagonalStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class BorderCollectionPropertyDiagonalStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get a cell and its style
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
// Set diagonal border properties
style.Borders.DiagonalStyle = CellBorderType.Thin;
style.Borders.DiagonalColor = Color.Red;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("DiagonalBorderDemo.xlsx");
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
