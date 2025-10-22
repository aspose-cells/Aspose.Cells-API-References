##HtmlSaveOptions.WidthScalable
HtmlSaveOptions property. Indicates whether exporting column width in unit of scale to html. The default value is false
## HtmlSaveOptions.WidthScalable property
Indicates whether exporting column width in unit of scale to html. The default value is false.
```csharp
public bool WidthScalable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyWidthScalableDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
worksheet.Cells["B1"].PutValue(123.45);
// Set HTML save options with WidthScalable property
HtmlSaveOptions options = new HtmlSaveOptions();
options.WidthScalable = true; // Demonstrate setting to true
// Save with scalable width
workbook.Save("output_scalable.html", options);
// Save again with fixed width
options.WidthScalable = false;
workbook.Save("output_fixed.html", options);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
