##TxtSaveOptions.TrimTailingBlankCells
TxtSaveOptions property. Indicates whether tailing blank cells in one row should be trimmed. Default is false
## TxtSaveOptions.TrimTailingBlankCells property
Indicates whether tailing blank cells in one row should be trimmed. Default is false.
```csharp
public bool TrimTailingBlankCells { get; set; }
```
### Remarks
When saving with LightCells mode and the [`ExportArea`](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [`LightCellsDataProvider`](../lightcellsdataprovider/)
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Add sample data
cells[0, 0].PutValue("A");
cells[0, 1].PutValue("B");
cells[0, 2].PutValue("C");
cells[1, 0].PutValue(1);
cells[1, 2].PutValue(2);
cells[2, 0].PutValue(3);
// Save without trimming trailing blank cells (default)
TxtSaveOptions options1 = new TxtSaveOptions
{
Encoding = Encoding.ASCII,
TrimTailingBlankCells = false
};
string result1 = SaveAsCsv(workbook, options1);
Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);
// Save with trimming trailing blank cells
TxtSaveOptions options2 = new TxtSaveOptions
{
Encoding = Encoding.ASCII,
TrimTailingBlankCells = true
};
string result2 = SaveAsCsv(workbook, options2);
Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
}
private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
{
using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
{
workbook.Save(stream, options);
return Encoding.ASCII.GetString(stream.ToArray());
}
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
