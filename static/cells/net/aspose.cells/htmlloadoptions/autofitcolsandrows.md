##HtmlLoadOptions.AutoFitColsAndRows
HtmlLoadOptions property. Indicates whether autofit columns and rows. The default value is false
## HtmlLoadOptions.AutoFitColsAndRows property
Indicates whether auto-fit columns and rows. The default value is false.
```csharp
public bool AutoFitColsAndRows { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
// Enable auto-fitting of columns and rows
loadOptions.AutoFitColsAndRows = true;
// Load HTML file with the specified options
Workbook workbook = new Workbook("example.html", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Auto-fit columns and rows will be applied during load
Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
