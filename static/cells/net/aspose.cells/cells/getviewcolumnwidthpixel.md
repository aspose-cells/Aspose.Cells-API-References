##Cells.GetViewColumnWidthPixel
Cells method. Get the width in different view type
## Cells.GetViewColumnWidthPixel method
Get the width in different view type.
```csharp
public int GetViewColumnWidthPixel(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
### Return Value
the column width in unit of pixels
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the view type to PageLayoutView
worksheet.ViewType = ViewType.PageLayoutView;
// Set column width in characters (will be converted to pixels)
worksheet.Cells.SetColumnWidth(0, 10);
// Get the column width in pixels
int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
// Output the result
Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
// Save the workbook
workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
