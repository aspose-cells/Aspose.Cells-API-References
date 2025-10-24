##Cells.GetRowHeightPixel
Cells method. Gets the height of a specified row in unit of pixel
## Cells.GetRowHeightPixel method
Gets the height of a specified row in unit of pixel.
```csharp
public int GetRowHeightPixel(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
Height of row
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetRowHeightPixelWithInt32Demo
{
public static void Run()
{
// Instantiate a new Workbook
Workbook wb = new Workbook();
// Get the first worksheet
Worksheet worksheet = wb.Worksheets[0];
// Set row height for row 5 (in pixels)
worksheet.Cells.SetRowHeightPixel(5, 30);
// Get row height for row 5 (in pixels)
int rowHeight = worksheet.Cells.GetRowHeightPixel(5);
Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
