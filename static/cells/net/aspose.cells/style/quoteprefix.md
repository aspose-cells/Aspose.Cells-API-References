##Style.QuotePrefix
Style property. Indicates whether the cells value starts with single quote mark
## Style.QuotePrefix property
Indicates whether the cell's value starts with single quote mark.
```csharp
public bool QuotePrefix { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyQuotePrefixDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B10 and set its value
Cell cell = worksheet.Cells["B10"];
cell.PutValue("'12345"); // Note the single quote prefix
// Get the cell's style and enable QuotePrefix
Style style = cell.GetStyle();
style.QuotePrefix = true;
cell.SetStyle(style);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the QuotePrefix property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
