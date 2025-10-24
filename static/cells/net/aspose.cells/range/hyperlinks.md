##Range.Hyperlinks
Range property. Gets all hyperlink in the range
## Range.Hyperlinks property
Gets all hyperlink in the range.
```csharp
public Hyperlink[] Hyperlinks { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyHyperlinksDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a hyperlink to cell A1
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Create a range containing A1
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
// Get hyperlinks in the range
Hyperlink[] hyperlinks = range.Hyperlinks;
// Display hyperlink information
if (hyperlinks.Length > 0)
{
Console.WriteLine("Hyperlink found:");
Console.WriteLine($"Address: {hyperlinks[0].Address}");
Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
// Delete the hyperlink
hyperlinks[0].Delete();
Console.WriteLine("Hyperlink deleted");
}
// Verify hyperlink was removed
Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
}
}
}
```
### See Also
* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
