##Spinner.CurrentValue
Spinner property. Gets or sets the current value
## Spinner.CurrentValue property
Gets or sets the current value.
```csharp
public int CurrentValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SpinnerPropertyCurrentValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a spinner control
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
Spinner spinner = (Spinner)shape;
// Set spinner properties
spinner.LinkedCell = "A1";
spinner.Min = 1;
spinner.Max = 100;
spinner.IncrementalChange = 5;
spinner.CurrentValue = 10; // Using CurrentValue property directly
// Verify and output the current value
Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);
// Save the workbook
workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
