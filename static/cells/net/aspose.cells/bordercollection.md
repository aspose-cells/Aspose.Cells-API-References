##Class BorderCollection
Aspose.Cells.BorderCollection class. Encapsulates a collection of Border objects
## BorderCollection class
Encapsulates a collection of [`Border`](../border/) objects.
```csharp
public class BorderCollection
```
## Properties
| Name | Description |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Gets or sets the Color of Diagonal lines. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Gets or sets the style of Diagonal lines. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Gets the [`Border`](../border/) element at the specified index. |
## Methods
| Name | Description |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Sets the Color of all borders in the collection. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Sets the style of all borders of the collection. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class BorderCollectionDemo
{
public static void BorderCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Workbook object
workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];
// Accessing the "A1" cell from the worksheet
Cell cell = worksheet.Cells["A1"];
// Adding some value to the "A1" cell
cell.PutValue("Visit Aspose!");
// Getting the style of the cell
Style style = cell.GetStyle();
// Setting the line style of the top border
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
// Setting the color of the top border
style.Borders[BorderType.TopBorder].Color = Color.Red;
// Setting the line style of the bottom border
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;
// Setting the color of the bottom border
style.Borders[BorderType.BottomBorder].Color = Color.Green;
// Setting the line style of the left border
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
// Setting the color of the left border
style.Borders[BorderType.LeftBorder].Color = Color.Yellow;
// Setting the line style of the right border
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;
// Setting the color of the right border
style.Borders[BorderType.RightBorder].Color = Color.Blue;
// Setting diagonal properties
style.Borders.DiagonalColor = Color.Red;
style.Borders.DiagonalStyle = CellBorderType.Dashed;
// Applying the style to the cell
cell.SetStyle(style);
// Saving the Excel file
workbook.Save("BorderCollectionExample.xlsx");
workbook.Save("BorderCollectionExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
