##SpreadsheetML2003SaveOptions.LimitAsXls
SpreadsheetML2003SaveOptions property. Limit as xls the max row index is 65535 and the max column index is 255
## SpreadsheetML2003SaveOptions.LimitAsXls property
Limit as xls, the max row index is 65535 and the max column index is 255.
```csharp
public bool LimitAsXls { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook(FileFormatType.Xlsx);
// Access cells and create a range
Cells cells = workbook.Worksheets[0].Cells;
Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
range.Name = "TestRange";
// Save with LimitAsXls = true
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
{
LimitAsXls = true
};
// Save as SpreadsheetML with XLS limits
workbook.Save("output.xml", saveOptions);
Console.WriteLine("File saved with LimitAsXls=true");
}
}
}
```
### See Also
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
