##CellsFactory.CreateStyle
CellsFactory method. Creates a new style
## CellsFactory.CreateStyle method
Creates a new style.
```csharp
public Style CreateStyle()
```
### Return Value
Returns a style object.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellsFactoryMethodCreateStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a style using CellsFactory
Style style = new CellsFactory().CreateStyle();
// Set border properties for the style
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
// Apply the style to a cell
workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
workbook.Worksheets[0].Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
