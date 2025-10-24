##BorderCollection.SetColor
BorderCollection method. Sets the Color of all borders in the collection
## BorderCollection.SetColor method
Sets the Color of all borders in the collection.
```csharp
public void SetColor(Color color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Borders' Color. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BorderCollectionMethodSetColorWithColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with colored borders
Style style = workbook.CreateStyle();
// Set border line styles
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
// Set border color to red using SetColor method
style.Borders.SetColor(Color.Red);
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Cell with colored borders");
cell.SetStyle(style);
// Auto-fit column for better visibility
worksheet.AutoFitColumn(0);
// Save the workbook
workbook.Save("BorderColorDemo.xlsx");
}
}
}
```
### See Also
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
