##Cells.StandardWidthPixels
Cells property. Gets or sets the default column width in the worksheet in unit of pixels
## Cells.StandardWidthPixels property
Gets or sets the default column width in the worksheet, in unit of pixels.
```csharp
public int StandardWidthPixels { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardWidthPixelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set and get the standard width in pixels
cells.StandardWidthPixels = 104;
Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);
// Set and get the standard width in characters
cells.StandardWidth = 12.375;
Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);
// Set and get the standard height in points
cells.StandardHeight = 14.25;
Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
