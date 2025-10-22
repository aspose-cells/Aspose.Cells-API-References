##ExportTableOptions.SkipErrorValue
ExportTableOptions property. Indicates whether skip invalid value for the column. For exampleif the column type is decimal the value is greater than decimal.MaxValue and this property is truewe will not throw exception again. The default value is false
## ExportTableOptions.SkipErrorValue property
Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false.
```csharp
public bool SkipErrorValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Data;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertySkipErrorValueDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.Germany;
Worksheet ws = wb.Worksheets[0];
// First test case - numeric values
ws.Cells["A1"].Value = "Double";
ws.Cells["A2"].Value = 1.56;
ExportTableOptions eto = new ExportTableOptions();
eto.ExportColumnName = true;
eto.SkipErrorValue = true;
eto.CheckMixedValueType = true;
DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56
// Second test case - mixed values
ws.Cells["A2"].Value = "dummy";
ws.Cells["A3"].Value = 1.56;
data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
// Third test case - export as string
data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
