##BorderCollection.SetStyle
BorderCollection method. Sets the style of all borders of the collection
## BorderCollection.SetStyle method
Sets the style of all borders of the collection.
```csharp
public void SetStyle(CellBorderType style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | CellBorderType | Borders' style |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get cell C6 and its style
Cell cell = worksheet.Cells["C6"];
Style style = cell.GetStyle();
// Set border color and style
style.Borders.SetColor(System.Drawing.Color.Red);
style.Borders.SetStyle(CellBorderType.Thick);
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");
Console.WriteLine("Border style set successfully.");
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
