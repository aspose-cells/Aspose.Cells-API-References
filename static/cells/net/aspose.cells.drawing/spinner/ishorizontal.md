##Spinner.IsHorizontal
Spinner property. Indicates whether this is a horizontal scroll bar
## Spinner.IsHorizontal property
Indicates whether this is a horizontal scroll bar.
```csharp
public bool IsHorizontal { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class SpinnerPropertyIsHorizontalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Add a spinner shape to the worksheet
Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
// Set spinner properties
spinner.Min = 0;
spinner.Max = 100;
spinner.IncrementalChange = 5;
spinner.CurrentValue = 50;
// Demonstrate IsHorizontal property (read and write)
Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
// Toggle the orientation
spinner.IsHorizontal = !spinner.IsHorizontal;
Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
// Save the workbook
workbook.Save("SpinnerIsHorizontalDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
