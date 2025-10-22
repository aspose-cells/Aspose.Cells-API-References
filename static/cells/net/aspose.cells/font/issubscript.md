##Font.IsSubscript
Font property. Gets or sets a value indicating whether the font is subscript
## Font.IsSubscript property
Gets or sets a value indicating whether the font is subscript.
```csharp
public bool IsSubscript { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsSubscriptDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with subscript text
Style subscriptStyle = workbook.CreateStyle();
subscriptStyle.Font.IsSubscript = true;
// Create a style with superscript text for comparison
Style superscriptStyle = workbook.CreateStyle();
superscriptStyle.Font.IsSuperscript = true;
// Apply styles to cells
worksheet.Cells["A1"].PutValue("Subscript Text");
worksheet.Cells["A1"].SetStyle(subscriptStyle);
worksheet.Cells["A2"].PutValue("Superscript Text");
worksheet.Cells["A2"].SetStyle(superscriptStyle);
// Verify and display the styles
Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);
// Save the workbook
workbook.Save("FontPropertyIsSubscriptDemo.ods");
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
