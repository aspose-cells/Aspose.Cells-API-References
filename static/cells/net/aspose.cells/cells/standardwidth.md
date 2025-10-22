##Cells.StandardWidth
Cells property. Gets or sets the default column width in the worksheet in unit of characters
## Cells.StandardWidth property
Gets or sets the default column width in the worksheet, in unit of characters.
```csharp
public double StandardWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set the standard width for columns
cells.StandardWidth = 18.25;
// Display the standard width and actual width of the first column
Console.WriteLine("Standard Width: " + cells.StandardWidth);
Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));
// Verify the standard width is applied (approximately)
if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
{
Console.WriteLine("Warning: Column width differs significantly from standard width");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
