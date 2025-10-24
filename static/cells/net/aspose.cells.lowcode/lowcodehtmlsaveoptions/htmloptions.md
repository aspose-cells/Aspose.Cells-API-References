##LowCodeHtmlSaveOptions.HtmlOptions
LowCodeHtmlSaveOptions property. The general options for saving html
## LowCodeHtmlSaveOptions.HtmlOptions property
The general options for saving html.
```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```
### Remarks
When one [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) instance is specified, the [`SaveFormat`](../saveformat/) will be overwritten(if it had been specified before).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.99);
// Create low-code HTML save options
LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
{
SaveFormat = SaveFormat.Html,
HtmlOptions = new HtmlSaveOptions()
};
// Display current gridlines export setting
Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);
// Save with gridlines visible
workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);
// Modify HTML options to hide gridlines
saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);
// Save without gridlines
workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);
Console.WriteLine("Demo executed successfully. Compare output files.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
