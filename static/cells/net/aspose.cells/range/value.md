##Range.Value
Range property. Gets and sets the value of the range
## Range.Value property
Gets and sets the value of the range.
```csharp
public object Value { get; set; }
```
### Remarks
If the range contains multiple cells, the returned/applied object should be a two-dimension Array object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range starting from A1 covering 3x3 cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
// Set a 2D array as the value for the range
int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
range.Value = values;
// Save the workbook
workbook.Save("RangePropertyValueDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
