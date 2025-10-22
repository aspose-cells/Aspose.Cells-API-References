##Cell.ContainsExternalLink
Cell property. Indicates whether this cell contains an external link. Only applies when the cell is a formula cell
## Cell.ContainsExternalLink property
Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.
```csharp
public bool ContainsExternalLink { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyContainsExternalLinkDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data and external link
sheet.Cells["A1"].PutValue("External Link:");
sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
// Check if cells contain external links
Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
