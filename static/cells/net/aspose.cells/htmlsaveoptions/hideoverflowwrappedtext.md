##HtmlSaveOptions.HideOverflowWrappedText
HtmlSaveOptions property. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false
## HtmlSaveOptions.HideOverflowWrappedText property
Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false
```csharp
public bool HideOverflowWrappedText { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text in cell A1
worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
// Create and apply style with text wrapping
Style style = workbook.CreateStyle();
style.IsTextWrapped = true;
StyleFlag flag = new StyleFlag();
flag.WrapText = true;
// Get the cells collection and apply style
Cells cells = worksheet.Cells;
cells["A1"].SetStyle(style, flag);
// Set column width to make text wrap
cells.SetColumnWidth(0, 10);
// Create HTML save options and set HideOverflowWrappedText
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.HideOverflowWrappedText = true;
// Save workbook with HTML options
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
