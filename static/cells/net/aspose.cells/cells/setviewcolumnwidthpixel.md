##Cells.SetViewColumnWidthPixel
Cells method. Sets the width of the column in different view
## Cells.SetViewColumnWidthPixel method
Sets the width of the column in different view.
```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| pixels | Int32 | The width in unit of pixels. |
### Remarks
If the current view type is PageLayoutView, the column's width is same as printed width.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Set sample data
sheet.Cells[0, 0].Value = "Sample Text";
// Calculate pixel width (100 pixels in this example)
int pixelWidth = 100;
// Set column width in pixels
sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
