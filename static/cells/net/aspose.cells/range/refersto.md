##Range.RefersTo
Range property. Gets the ranges refers to
## Range.RefersTo property
Gets the range's refers to.
```csharp
public string RefersTo { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyRefersToDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Create a named range
int index = workbook.Worksheets.Names.Add("MyRange");
Name name = workbook.Worksheets.Names[index];
// Set the RefersTo property for the named range
name.RefersTo = "=Sheet1!$A$1:$A$3";
// Get the ranges referred by the name
Aspose.Cells.Range[] ranges = name.GetRanges();
// Display the RefersTo property of the first range
Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
// Create a formula that uses the named range
worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
// Calculate the formula
Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
