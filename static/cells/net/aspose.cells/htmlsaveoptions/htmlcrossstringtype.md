##HtmlSaveOptions.HtmlCrossStringType
HtmlSaveOptions property. Indicates if a crosscell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default so for crosscell strings there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html filessetting the value to Cross would be several times faster than setting it to Default or Fit2Cell
## HtmlSaveOptions.HtmlCrossStringType property
Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format. By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel. But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.
```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data that will demonstrate cross-string behavior
worksheet.Cells["A1"].PutValue("Left Content");
worksheet.Cells["B1"].PutValue("Right Content");
// Get and modify cell styles
Style styleA1 = worksheet.Cells["A1"].GetStyle();
styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
worksheet.Cells["A1"].SetStyle(styleA1);
Style styleB1 = worksheet.Cells["B1"].GetStyle();
styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
worksheet.Cells["B1"].SetStyle(styleB1);
// Configure HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
// Save the workbook to HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with CrossHideRight option.");
}
}
}
```
### See Also
* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
