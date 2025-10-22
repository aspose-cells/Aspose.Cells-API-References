##Style.Borders
Style property. Gets the BorderCollection of the style
## Style.Borders property
Gets the [`BorderCollection`](../../bordercollection/) of the style.
```csharp
public BorderCollection Borders { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyBordersDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get cell and its style
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
// Set different border styles
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
