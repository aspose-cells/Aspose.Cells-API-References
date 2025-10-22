##HtmlSaveOptions.HiddenRowDisplayType
HtmlSaveOptions property. Hidden rowthe height of this row is 0 in excelbefore save this into html format if HtmlHiddenRowDisplayType is Removethe hidden row would not been output if the value is Hidden the row would been outputbut was hiddenthe default value is Hidden
## HtmlSaveOptions.HiddenRowDisplayType property
Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"
```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and hide a row
worksheet.Cells["A1"].PutValue("Visible Row");
worksheet.Cells["A2"].PutValue("Hidden Row");
worksheet.Cells["A3"].PutValue("Visible Row");
worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)
// Set HTML save options with HiddenRowDisplayType
HtmlSaveOptions options = new HtmlSaveOptions();
options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
// Save to HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
}
}
}
```
### See Also
* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
