##Spinner.Max
Spinner property. Gets or sets the maximum value of a scroll bar or spinner range
## Spinner.Max property
Gets or sets the maximum value of a scroll bar or spinner range.
```csharp
public int Max { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpinnerPropertyMaxDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
spinner.Min = 0;
spinner.Max = 100;
spinner.IncrementalChange = 5;
Console.WriteLine($"Spinner Max Value: {spinner.Max}");
}
}
}
```
### See Also
* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
