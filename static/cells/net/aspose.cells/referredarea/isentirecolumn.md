##ReferredArea.IsEntireColumn
ReferredArea property. Indicates whether this area contains all rowsentire column
## ReferredArea.IsEntireColumn property
Indicates whether this area contains all rows(entire column).
```csharp
public bool IsEntireColumn { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ReferredAreaPropertyIsEntireColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
// Create a named range referring to entire column B
int index = workbook.Worksheets.Names.Add("PriceColumn");
workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";
// Get the referred area of the named range
ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];
// Display the IsEntireColumn property value
Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);
// Create another named range referring to a specific range (not entire column)
int index2 = workbook.Worksheets.Names.Add("ProductRange");
workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";
// Get the referred area of the second named range
ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];
// Display the IsEntireColumn property value for the second range
Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);
// Demonstrate the effect of IsEntireColumn by checking the range dimensions
Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);
Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);
// Save the workbook
workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
