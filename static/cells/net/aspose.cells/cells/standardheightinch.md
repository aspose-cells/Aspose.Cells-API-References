##Cells.StandardHeightInch
Cells property. Gets or sets the default row height in this worksheet in unit of inches
## Cells.StandardHeightInch property
Gets or sets the default row height in this worksheet, in unit of inches.
```csharp
public double StandardHeightInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStandardHeightInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the standard height in inches
double standardHeightInch = worksheet.Cells.StandardHeightInch;
Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
// Set a new standard height (1 inch)
worksheet.Cells.StandardHeightInch = 1.0;
Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
