##OoxmlSaveOptions.ExportCellName
OoxmlSaveOptions property. Indicates if export cell name to Excel2007 .xlsx .xlsm .xltx .xltm file. If the output file may be accessed by SQL Server DTS this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true
## OoxmlSaveOptions.ExportCellName property
Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.
```csharp
public bool ExportCellName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsPropertyExportCellNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Put some data in cells
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["B2"].PutValue(123);
// Create XLSX save options with ExportCellName enabled
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.ExportCellName = true;
// Save the workbook with cell names exported
workbook.Save("output_with_cellnames.xlsx", saveOptions);
// Create another save options with ExportCellName disabled (default)
OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
// Save the workbook without cell names exported
workbook.Save("output_without_cellnames.xlsx", saveOptions2);
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
