##Range.FirstRow
Range property. Gets the index of the first row of the range
## Range.FirstRow property
Gets the index of the first row of the range.
```csharp
public int FirstRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyFirstRowDemo
{
public static void Run()
{
// Create a workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
// Create a range
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
// Access and display FirstRow property
Console.WriteLine("First row index of range: " + range.FirstRow);
// Access the first cell in the first row of the range
Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
Console.WriteLine("First cell value: " + firstCell.StringValue);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
