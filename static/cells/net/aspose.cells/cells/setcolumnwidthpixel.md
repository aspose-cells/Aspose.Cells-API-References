##Cells.SetColumnWidthPixel
Cells method. Sets column width in unit of pixels in normal view
## Cells.SetColumnWidthPixel method
Sets column width in unit of pixels in normal view.
```csharp
public void SetColumnWidthPixel(int column, int pixels)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| pixels | Int32 | Number of pixels. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set column widths in pixels for columns 1 through 5
for (int i = 0; i < 5; i++)
{
cells.SetColumnWidthPixel(i, 120); // 120 pixels width
}
// Save the workbook
workbook.Save("SetColumnWidthPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
