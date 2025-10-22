##HtmlSaveOptions.ExportSimilarBorderStyle
HtmlSaveOptions property. Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel please keep the default value. The default value is false
## HtmlSaveOptions.ExportSimilarBorderStyle property
Indicating whether exporting the similar border style when the border style is not supported by browsers. If you want to import the html or mht file to excel, please keep the default value. The default value is false.
```csharp
public bool ExportSimilarBorderStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with borders
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
worksheet.Cells["B1"].PutValue("Similar Border");
worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
worksheet.Cells["C1"].PutValue("Different Border");
worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));
// Create HTML save options
HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
{
ExportSimilarBorderStyle = true // Demonstrate the property
};
// Save the workbook
workbook.Save("output.html", htmlSaveOptions);
}
private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
{
Style style = workbook.CreateStyle();
style.Borders[BorderType.TopBorder].LineStyle = borderType;
style.Borders[BorderType.BottomBorder].LineStyle = borderType;
style.Borders[BorderType.LeftBorder].LineStyle = borderType;
style.Borders[BorderType.RightBorder].LineStyle = borderType;
return style;
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
