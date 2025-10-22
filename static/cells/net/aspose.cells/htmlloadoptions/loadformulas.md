##HtmlLoadOptions.LoadFormulas
HtmlLoadOptions property. Indicates whether importing formulas if the original html file contains formulas
## HtmlLoadOptions.LoadFormulas property
Indicates whether importing formulas if the original html file contains formulas
```csharp
public bool LoadFormulas { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyLoadFormulasDemo
{
public static void Run()
{
// Create an instance of HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Set LoadFormulas to true to load formulas from HTML
loadOptions.LoadFormulas = true;
// Load an HTML file containing formulas into a Workbook
Workbook workbook = new Workbook("input.html", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display formula from cell A1 (if present in HTML)
Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);
// Save the workbook to an Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
