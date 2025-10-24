##UnionRange.RefersTo
UnionRange property. Gets the ranges refers to
## UnionRange.RefersTo property
Gets the range's refers to.
```csharp
public string RefersTo { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyRefersToDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(800);
// Create a named range
Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
namedRange.Name = "ProductPrices";
// Create a union range that includes our named range
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });
// Display the RefersTo property of the union range
Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);
// Create another range and display its RefersTo
Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);
// Demonstrate using RefersTo to identify range composition
Console.WriteLine("Does union range contain named range? " +
unionRange.RefersTo.Contains("ProductPrices"));
// Show how RefersTo changes when ranges are modified
Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);
// Save the workbook
workbook.Save("UnionRangeRefersToDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
