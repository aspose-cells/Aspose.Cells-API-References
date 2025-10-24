##HtmlSaveOptions.FormatDataIgnoreColumnWidth
HtmlSaveOptions property. Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property
Indicating whether show the whole formatted data of cell when overflowing the column. If true then ignore the column width and the whole data of cell will be exported. If false then the data will be exported same as Excel. The default value is false.
```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and column width
worksheet.Cells["A1"].PutValue("Sample Text");
worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Demonstrate FormatDataIgnoreColumnWidth property
saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
// Save with different settings to show the effect
workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
