##ReferredArea.SheetNames
ReferredArea property. Names of all the worksheets this instance references to
## ReferredArea.SheetNames property
Names of all the worksheets this instance references to.
```csharp
public string[] SheetNames { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ReferredAreaPropertySheetNamesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to create a formula reference
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Calculate formulas to get references
workbook.CalculateFormula();
// Get the referred area from the formula in A3
ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];
// Display the SheetNames property
Console.WriteLine("SheetNames referenced by the formula:");
if (referredArea.SheetNames != null)
{
foreach (string sheetName in referredArea.SheetNames)
{
Console.WriteLine(sheetName);
}
}
// Add another worksheet and create a cross-sheet reference
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
sheet2.Cells["B1"].PutValue("=Sheet1!A3");
// Calculate formulas again
workbook.CalculateFormula();
// Get the referred area from the cross-sheet formula
ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];
// Display SheetNames for cross-sheet reference
Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
if (crossSheetArea.SheetNames != null)
{
foreach (string sheetName in crossSheetArea.SheetNames)
{
Console.WriteLine(sheetName);
}
}
// Save the workbook
workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
