##BorderCollection.DiagonalColor
BorderCollection property. Gets or sets the Color of Diagonal lines
## BorderCollection.DiagonalColor property
Gets or sets the Color of Diagonal lines.
```csharp
public Color DiagonalColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class BorderCollectionPropertyDiagonalColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Diagonal Border Demo");
Style style = cell.GetStyle();
// Setting diagonal border properties
style.Borders.DiagonalColor = Color.Red;
style.Borders.DiagonalStyle = CellBorderType.Thick;
cell.SetStyle(style);
// Save the workbook
workbook.Save("DiagonalBorderDemo.xlsx");
}
}
}
```
### See Also
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
