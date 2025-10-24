##ProtectedRange.CellArea
ProtectedRange property. Gets the CellArea object represents the cell area to be protected
## ProtectedRange.CellArea property
Gets the `CellArea` object represents the cell area to be protected.
```csharp
public CellArea CellArea { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangePropertyCellAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create protected ranges
ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
// Add first protected range
int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
ProtectedRange range1 = allowRanges[index1];
range1.Password = "123";
// Add second protected range
int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
ProtectedRange range2 = allowRanges[index2];
range2.Password = "456";
// Display CellArea information for both ranges
Console.WriteLine("Protected Range 1:");
Console.WriteLine($"Name: {range1.Name}");
Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");
Console.WriteLine("\nProtected Range 2:");
Console.WriteLine($"Name: {range2.Name}");
Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");
// Save the workbook
workbook.Save("ProtectedRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
