##TxtSaveOptions.ExportAllSheets
TxtSaveOptions property. Indicates whether exporting all sheets to the text file. If it is false only export the activesheet just like MS Excel
## TxtSaveOptions.ExportAllSheets property
Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.
```csharp
public bool ExportAllSheets { get; set; }
```
### Remarks
The defult value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyExportAllSheetsDemo
{
public static void Run()
{
// Create a workbook with two sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Add sample data to both sheets
workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
workbook.Worksheets[0].Cells["A2"].PutValue(1);
workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
workbook.Worksheets[1].Cells["A2"].PutValue(2);
// Save with ExportAllSheets=false (default)
TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
workbook.Save("output_single_sheet.csv", saveOptions);
// Save with ExportAllSheets=true
saveOptions.ExportAllSheets = true;
workbook.Save("output_all_sheets.csv", saveOptions);
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
