##ExportTableOptions.ExportAsHtmlString
ExportTableOptions property. Exports the html string value of the cells to the DataTable
## ExportTableOptions.ExportAsHtmlString property
Exports the html string value of the cells to the DataTable.
```csharp
public bool ExportAsHtmlString { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyExportAsHtmlStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set cell value with formatting
cells["A1"].PutValue("abc");
Style style = cells["A1"].GetStyle();
style.Font.Name = "Arial";
style.Font.Size = 10;
style.Font.Color = System.Drawing.Color.Black;
cells["A1"].SetStyle(style);
// Export with ExportAsHtmlString
ExportTableOptions etOpt = new ExportTableOptions();
etOpt.ExportColumnName = false;
etOpt.ExportAsHtmlString = true;
DataTable dt = cells.ExportDataTable(0, 0, 1, 1, etOpt);
Console.WriteLine("HTML String: " + dt.Rows[0][0].ToString());
Console.WriteLine("Expected Format: " + cells["A1"].HtmlString);
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
