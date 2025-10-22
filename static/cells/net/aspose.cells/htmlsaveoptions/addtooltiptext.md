##HtmlSaveOptions.AddTooltipText
HtmlSaveOptions property. Indicates whether adding tooltip text when the data cant be fully displayed. The default value is false
## HtmlSaveOptions.AddTooltipText property
Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.
```csharp
public bool AddTooltipText { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyAddTooltipTextDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a long text that will exceed cell width
worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
// Configure HTML save options with tooltip
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
saveOptions.AddTooltipText = true;
// Save the workbook
string outputPath = "output_with_tooltip.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("File saved with tooltips: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
