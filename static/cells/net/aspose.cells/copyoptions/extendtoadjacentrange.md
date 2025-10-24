##CopyOptions.ExtendToAdjacentRange
CopyOptions property. Indicates whether extend ranges when copying the range to adjacent range
## CopyOptions.ExtendToAdjacentRange property
Indicates whether extend ranges when copying the range to adjacent range.
```csharp
public bool ExtendToAdjacentRange { get; set; }
```
### Remarks
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyExtendToAdjacentRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add a hyperlink to cell A1
ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Create copy options and set ExtendToAdjacentRange to true
CopyOptions copyOptions = new CopyOptions();
copyOptions.ExtendToAdjacentRange = true;
// Copy row 0 to row 1 with the copy options
ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);
// Verify the hyperlink was extended to the adjacent range
Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
