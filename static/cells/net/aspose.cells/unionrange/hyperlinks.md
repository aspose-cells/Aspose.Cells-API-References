##UnionRange.Hyperlinks
UnionRange property. Gets all hyperlink in the range
## UnionRange.Hyperlinks property
Gets all hyperlink in the range.
```csharp
public Hyperlink[] Hyperlinks { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyHyperlinksDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some hyperlinks to cells
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");
// Create a range
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });
// Get hyperlinks in the range
Hyperlink[] hyperlinks = unionRange.Hyperlinks;
Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);
// Display information about each hyperlink
foreach (Hyperlink link in hyperlinks)
{
Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
}
// Save the workbook
workbook.Save("HyperlinksDemo.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
