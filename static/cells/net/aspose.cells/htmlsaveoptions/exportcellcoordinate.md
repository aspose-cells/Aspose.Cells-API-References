##HtmlSaveOptions.ExportCellCoordinate
HtmlSaveOptions property. Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel please keep the default value
## HtmlSaveOptions.ExportCellCoordinate property
Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false. If you want to import the output html to excel, please keep the default value.
```csharp
public bool ExportCellCoordinate { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Create HTML save options and enable ExportCellCoordinate
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportCellCoordinate = true;
// Save the workbook as HTML with cell coordinates
workbook.Save("output.html", options);
Console.WriteLine("HTML with cell coordinates exported successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
