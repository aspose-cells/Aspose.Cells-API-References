##SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell
SpreadsheetML2003SaveOptions property. The default value is false it means that column index will be ignored if the cell is contiguous to the previous cell
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property
The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell.
```csharp
public bool ExportColumnIndexOfCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Create save options with ExportColumnIndexOfCell enabled
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
saveOptions.ExportColumnIndexOfCell = true;
// Save the workbook with column index information
workbook.Save("output_with_column_index.xml", saveOptions);
Console.WriteLine("File saved with column index information.");
}
}
}
```
### See Also
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
