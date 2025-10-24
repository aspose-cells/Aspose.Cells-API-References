##Spinner.IncrementalChange
Spinner property. Gets or sets the amount that the scroll bar or spinner is incremented a line scroll
## Spinner.IncrementalChange property
Gets or sets the amount that the scroll bar or spinner is incremented a line scroll.
```csharp
public int IncrementalChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SpinnerPropertyIncrementalChangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a spinner control
Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);
// Set spinner properties
spinner.Min = 0;
spinner.Max = 100;
spinner.CurrentValue = 50;
spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property
// Verify and output the IncrementalChange value
Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);
// Modify and verify again
spinner.IncrementalChange = 10;
Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);
// Save the workbook
workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
