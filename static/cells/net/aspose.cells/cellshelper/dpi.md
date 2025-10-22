##CellsHelper.DPI
CellsHelper property. Gets the DPI of the machine
## CellsHelper.DPI property
Gets the DPI of the machine.
```csharp
public static double DPI { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyDPIDemo
{
public static void Run()
{
// Set and display current DPI
Console.WriteLine("Original DPI: " + CellsHelper.DPI);
// Change DPI setting
CellsHelper.DPI = 300;
Console.WriteLine("New DPI: " + CellsHelper.DPI);
// Create a new workbook and save with different DPI settings
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample shape to demonstrate DPI effect
sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);
// Save with current DPI setting
workbook.Save("output_with_dpi_300.xlsx");
// Change DPI and save again
CellsHelper.DPI = 96;
workbook.Save("output_with_dpi_96.xlsx");
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
