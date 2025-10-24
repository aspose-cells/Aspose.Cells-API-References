##Range.Address
Range property. Gets address of the range
## Range.Address property
Gets address of the range.
```csharp
public string Address { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyAddressDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a range and demonstrate Address property
Aspose.Cells.Range range = cells.CreateRange("A1");
Console.WriteLine("Original range address: " + range.Address);
// Demonstrate GetOffset with Address
Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
Console.WriteLine("Offset range address: " + offsetRange.Address);
// Demonstrate EntireRow Address
Aspose.Cells.Range entireRow = range.EntireRow;
Console.WriteLine("Entire row address: " + entireRow.Address);
// Demonstrate EntireColumn Address
Aspose.Cells.Range entireColumn = range.EntireColumn;
Console.WriteLine("Entire column address: " + entireColumn.Address);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
