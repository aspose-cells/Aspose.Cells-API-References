##FindOptions.IsRangeSet
FindOptions property. Indicates whether the searched range is set
## FindOptions.IsRangeSet property
Indicates whether the searched range is set.
```csharp
public bool IsRangeSet { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FindOptionsPropertyIsRangeSetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Cherry");
worksheet.Cells["B1"].PutValue("Date");
worksheet.Cells["B2"].PutValue("Elderberry");
worksheet.Cells["B3"].PutValue("Fig");
// Create FindOptions instance
FindOptions findOptions = new FindOptions();
// Check initial IsRangeSet value (should be false)
Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);
// Set a search range
CellArea searchRange = new CellArea();
searchRange.StartRow = 0;
searchRange.StartColumn = 0;
searchRange.EndRow = 2;
searchRange.EndColumn = 0; // Column A only
findOptions.SetRange(searchRange);
// Check IsRangeSet after setting range (should be true)
Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);
// Perform a find operation within the specified range
Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);
// Try to find something outside the range (should not be found)
foundCell = worksheet.Cells.Find("Fig", null, findOptions);
Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null
// Save the workbook
workbook.Save("PropertyIsRangeSetDemo.xlsx");
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
