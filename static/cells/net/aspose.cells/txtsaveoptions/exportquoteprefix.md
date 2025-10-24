##TxtSaveOptions.ExportQuotePrefix
TxtSaveOptions property. Indicates whether the single quote sign should be exported as part of the value of one cell when QuotePrefix is true for it. Default is false
## TxtSaveOptions.ExportQuotePrefix property
Indicates whether the single quote sign should be exported as part of the value of one cell when [`QuotePrefix`](../../style/quoteprefix/) is true for it. Default is false.
```csharp
public bool ExportQuotePrefix { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyExportQuotePrefixDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Add sample data with special characters
cells[0, 0].PutValue("a\\bcdef\"g");
cells[0, 1].PutValue("f\"g");
cells[0, 2].PutValue("a\\bcdg");
cells[0, 3].PutValue("abcdefg");
cells[0, 4].PutValue("efg");
cells[0, 5].PutValue("'abc");
// Create TXT save options
TxtSaveOptions saveOptions = new TxtSaveOptions
{
Encoding = Encoding.ASCII,
Separator = ',',
ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
};
// Save with ExportQuotePrefix = true
workbook.Save("output_with_exportquoteprefix.csv", saveOptions);
// Change separator and save again
saveOptions.Separator = '\\';
workbook.Save("output_with_backslash_separator.csv", saveOptions);
Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
