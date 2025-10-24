##LowCodeHtmlSaveOptions.SaveFormat
LowCodeHtmlSaveOptions property. Gets and sets the format of spreadsheet
## LowCodeHtmlSaveOptions.SaveFormat property
Gets and sets the format of spreadsheet.
```csharp
public override SaveFormat SaveFormat { get; set; }
```
### Remarks
When changing this property, the save format specified by [`HtmlOptions`](../htmloptions/) will be ignored(if it had been specified before).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Export");
LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);
options.SaveFormat = SaveFormat.Html;
options.HtmlOptions = new HtmlSaveOptions();
workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
