##HtmlLoadOptions.SupportDivTag
HtmlLoadOptions property. Indicates whether support the layout of div tag when the html file contains it. The default value is false
## HtmlLoadOptions.SupportDivTag property
Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.
```csharp
public bool SupportDivTag { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertySupportDivTagDemo
{
public static void Run()
{
// Create HTML load options with SupportDivTag enabled
HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
htmlLoadOptions.SupportDivTag = true;
// Load HTML file with div tags
Workbook workbook = new Workbook("input.html", htmlLoadOptions);
// Access data from the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
// Output cell value and style information
Console.WriteLine("Cell A1 value: " + cell.StringValue);
Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);
// Save as Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
