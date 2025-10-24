##HtmlLoadOptions.HasFormula
HtmlLoadOptions property. Indicates whether the text is formula if it starts with
## HtmlLoadOptions.HasFormula property
Indicates whether the text is formula if it starts with "=".
```csharp
public bool HasFormula { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyHasFormulaDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
// Set HasFormula to false to treat formula strings as plain text
loadOptions.HasFormula = false;
// Create workbook with HTML file and load options
Workbook workbook = new Workbook("example.html", loadOptions);
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Display some cell values to demonstrate HTML import
Console.WriteLine("A1: " + cells["A1"].StringValue);
Console.WriteLine("B1: " + cells["B1"].StringValue);
// Save as XLSX
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
