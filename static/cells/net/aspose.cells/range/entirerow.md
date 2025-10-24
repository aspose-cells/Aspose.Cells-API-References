##Range.EntireRow
Range property. Gets a Range object that represents the entire row or rows that contains the specified range
## Range.EntireRow property
Gets a Range object that represents the entire row (or rows) that contains the specified range.
```csharp
public Range EntireRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyEntireRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Fill some sample data in the first row
for (int col = 0; col < 5; col++)
{
sheet.Cells[0, col].PutValue($"Header {col + 1}");
}
// Get the entire first row using EntireRow property
Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;
// Copy the first row to the third row
Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
destination.Copy(entireRow);
// Save the workbook
workbook.Save("EntireRowDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
