##TxtSaveOptions.KeepSeparatorsForBlankRow
TxtSaveOptions property. Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty
## TxtSaveOptions.KeepSeparatorsForBlankRow property
Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.
```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Add some data with blank rows
cells[0, 0].PutValue("a");
cells[0, 1].PutValue("b");
cells[3, 0].PutValue("c");
cells[4, 1].PutValue("d");
// Create save options with KeepSeparatorsForBlankRow set to true
TxtSaveOptions options = new TxtSaveOptions
{
Encoding = Encoding.ASCII,
KeepSeparatorsForBlankRow = true
};
// Save the workbook to CSV with the options
string csvOutput = SaveAsCsv(wb, options);
Console.WriteLine(csvOutput);
}
private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
{
using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
{
wb.Save(stream, options);
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
