##Cell.Type
Cell property. Represents cell value type
## Cell.Type property
Represents cell value type.
```csharp
public CellValueType Type { get; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.USA;
Cells cells = wb.Worksheets[0].Cells;
// Demonstrate Type property with different values
cells["A1"].PutValue("123.45");
Console.WriteLine($"A1 Type: {cells["A1"].Type}"); // Should be IsNumeric
cells["A2"].PutValue("Hello");
Console.WriteLine($"A2 Type: {cells["A2"].Type}"); // Should be IsString
cells["A3"].PutValue(DateTime.Now);
Console.WriteLine($"A3 Type: {cells["A3"].Type}"); // Should be IsDateTime
cells["A4"].PutValue(true);
Console.WriteLine($"A4 Type: {cells["A4"].Type}"); // Should be IsBool
// Demonstrate with different regional settings
Cells sheet2Cells = wb.Worksheets.Add("Sheet2").Cells;
TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
tlo.Region = CountryCode.Germany;
using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes("\"1,2345\",\"12.345\"")))
{
sheet2Cells.ImportCSV(ms, tlo, 0, 0);
Console.WriteLine($"Sheet2 A1 Type: {sheet2Cells["A1"].Type}"); // Should be IsNumeric (German decimal)
Console.WriteLine($"Sheet2 B1 Type: {sheet2Cells["B1"].Type}"); // Should be IsString
}
}
}
}
```
### See Also
* enum [CellValueType](../../cellvaluetype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
