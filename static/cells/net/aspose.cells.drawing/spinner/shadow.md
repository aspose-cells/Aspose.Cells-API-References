##Spinner.Shadow
Spinner property. Indicates whether the shape has 3D shading
## Spinner.Shadow property
Indicates whether the shape has 3-D shading.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SpinnerPropertyShadowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a spinner to the worksheet
Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
// Set spinner properties
spinner.Min = 0;
spinner.Max = 100;
spinner.IncrementalChange = 5;
spinner.CurrentValue = 50;
// Demonstrate Shadow property
spinner.Shadow = true; // Enable 3D shadow effect
Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);
// Save the workbook
workbook.Save("SpinnerShadowDemo.xlsx");
// Load the saved workbook to verify shadow property
Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
