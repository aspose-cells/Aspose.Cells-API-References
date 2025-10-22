##HtmlSaveOptions.ExcludeUnusedStyles
HtmlSaveOptions property. Indicating whether excludes unused styles. For the generated html files excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated htmlsuch as the scenario that user needs to restore the workbook from the generated html later please set this property as false
## HtmlSaveOptions.ExcludeUnusedStyles property
Indicating whether excludes unused styles. For the generated html files, excluding unused styles can make the file size smaller without affecting the visual effects. So the default value of this property is true. If user needs to keep all styles in the workbook for the generated html(such as the scenario that user needs to restore the workbook from the generated html later), please set this property as false.
```csharp
public bool ExcludeUnusedStyles { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add sample data with different styles
Cell cell1 = workbook.Worksheets[0].Cells["A1"];
cell1.Value = "Styled text";
Style style1 = cell1.GetStyle();
style1.Font.Color = Color.Red;
style1.Font.IsBold = true;
cell1.SetStyle(style1);
Cell cell2 = workbook.Worksheets[0].Cells["A2"];
cell2.Value = "Different style";
Style style2 = cell2.GetStyle();
style2.Font.Name = "Times New Roman";
style2.Font.Size = 14;
cell2.SetStyle(style2);
// Configure HTML save options to exclude unused styles
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExcludeUnusedStyles = true;
// Save the workbook with HTML options
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
