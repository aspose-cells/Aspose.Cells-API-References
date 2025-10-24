##Spinner.Min
Spinner property. Gets or sets the minimum value of a scroll bar or spinner range
## Spinner.Min property
Gets or sets the minimum value of a scroll bar or spinner range.
```csharp
public int Min { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SpinnerPropertyMinDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a spinner control with proper dimensions
Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);
// Set spinner properties including Min
spinner.Min = 10;
spinner.Max = 100;
spinner.IncrementalChange = 5;
spinner.CurrentValue = 15;
// Verify and output the Min property
Console.WriteLine("Spinner Min Value: " + spinner.Min);
// Save the workbook
workbook.Save("SpinnerPropertyMinDemo.xlsx");
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
