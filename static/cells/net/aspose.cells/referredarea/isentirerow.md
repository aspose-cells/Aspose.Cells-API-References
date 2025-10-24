##ReferredArea.IsEntireRow
ReferredArea property. Indicates whether this area contains all columnsentire row
## ReferredArea.IsEntireRow property
Indicates whether this area contains all columns(entire row).
```csharp
public bool IsEntireRow { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ReferredAreaPropertyIsEntireRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["A3"].PutValue(300);
worksheet.Cells["B3"].PutValue(400);
// Create a named range referring to entire row 2
int index1 = workbook.Worksheets.Names.Add("NamedRange1");
workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";
// Get the referred area of the named range
ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];
// Display the current value of IsEntireRow
Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);
// Create another named range referring to a specific range (not entire row)
int index2 = workbook.Worksheets.Names.Add("NamedRange2");
workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";
// Get the referred area of the second named range
ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];
// Display the current value of IsEntireRow for the second range
Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);
// Demonstrate the effect of IsEntireRow by checking the range dimensions
Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);
Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);
// Save the workbook
workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
