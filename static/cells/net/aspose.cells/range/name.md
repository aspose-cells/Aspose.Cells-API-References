##Range.Name
Range property. Gets or sets the name of the range
## Range.Name property
Gets or sets the name of the range.
```csharp
public string Name { get; set; }
```
### Remarks
Named range is supported. For example,
range.Name = "Sheet1!MyRange";
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a range (columns A to B)
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
// Set the name property for the range
range.Name = "testRange";
// Verify the name was set
Console.WriteLine("Range name: " + range.Name);
// Save the workbook
workbook.Save("RangeWithName.xlsx");
// Open the saved file to demonstrate the name persists
Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
Console.WriteLine("Loaded range name: " + loadedRange.Name);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
