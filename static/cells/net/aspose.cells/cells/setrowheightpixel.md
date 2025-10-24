##Cells.SetRowHeightPixel
Cells method. Sets row height in unit of pixels
## Cells.SetRowHeightPixel method
Sets row height in unit of pixels.
```csharp
public void SetRowHeightPixel(int row, int pixels)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| pixels | Int32 | Number of pixels. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set height of first row to 50 pixels
worksheet.Cells.SetRowHeightPixel(0, 50);
// Set height of second row to 100 pixels
worksheet.Cells.SetRowHeightPixel(1, 100);
// Save the workbook
workbook.Save("RowHeightPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
