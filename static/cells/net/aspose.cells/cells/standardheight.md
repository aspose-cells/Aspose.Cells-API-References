##Cells.StandardHeight
Cells property. Gets or sets the default row height in this worksheet in unit of points
## Cells.StandardHeight property
Gets or sets the default row height in this worksheet, in unit of points.
```csharp
public double StandardHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get and display the standard height
double standardHeight = worksheet.Cells.StandardHeight;
Console.WriteLine("Standard Height: " + standardHeight);
// Set a new standard height
worksheet.Cells.StandardHeight = 20;
Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
// Save the workbook
workbook.Save("StandardHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
