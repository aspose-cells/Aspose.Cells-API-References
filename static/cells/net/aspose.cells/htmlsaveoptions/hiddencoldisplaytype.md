##HtmlSaveOptions.HiddenColDisplayType
HtmlSaveOptions property. Hidden columnthe width of this column is 0 in excelbefore save this into html format if HtmlHiddenColDisplayType is Removethe hidden column would not been output if the value is Hidden the column would been outputbut was hiddenthe default value is Hidden
## HtmlSaveOptions.HiddenColDisplayType property
Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"
```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Hide column C (index 2)
worksheet.Cells.HideColumn(2);
// Add some data to demonstrate
worksheet.Cells["A1"].PutValue("Visible Column A");
worksheet.Cells["B1"].PutValue("Visible Column B");
worksheet.Cells["C1"].PutValue("Hidden Column C");
worksheet.Cells["D1"].PutValue("Visible Column D");
// Create HTML save options with different HiddenColDisplayType settings
HtmlSaveOptions optionsRemove = new HtmlSaveOptions
{
HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
};
HtmlSaveOptions optionsHidden = new HtmlSaveOptions
{
HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
};
// Save with different options
workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
}
}
}
```
### See Also
* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
