##LoadOptions.LoadFormat
LoadOptions property. Gets the load format
## LoadOptions.LoadFormat property
Gets the load format.
```csharp
public LoadFormat LoadFormat { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class LoadOptionsPropertyLoadFormatDemo
{
public static void Run()
{
// Create sample CSV file
File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");
// Create LoadOptions for CSV format and display property
LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);
// Load CSV with correct options
Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);
// Create LoadOptions for XLSX format and display property
LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);
// Create/save sample XLSX file
Workbook newWorkbook = new Workbook();
newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
newWorkbook.Save("sample.xlsx");
// Load XLSX with correct options
Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);
// Cleanup temporary files
File.Delete("sample.csv");
File.Delete("sample.xlsx");
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
