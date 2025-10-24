##PasteOptions.SkipBlanks
PasteOptions property. Indicates whether skips blank cells
## PasteOptions.SkipBlanks property
Indicates whether skips blank cells.
```csharp
public bool SkipBlanks { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertySkipBlanksDemo
{
public static void Run()
{
// Create a source workbook with sample data
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Fill source range with some values and blanks
sourceSheet.Cells["A1"].PutValue("Value 1");
sourceSheet.Cells["A2"].PutValue(""); // Blank cell
sourceSheet.Cells["A3"].PutValue("Value 3");
sourceSheet.Cells["A4"].PutValue(""); // Blank cell
// Create destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Fill destination range with existing values
destSheet.Cells["A1"].PutValue("Existing 1");
destSheet.Cells["A2"].PutValue("Existing 2");
destSheet.Cells["A3"].PutValue("Existing 3");
destSheet.Cells["A4"].PutValue("Existing 4");
// Get ranges with fully qualified type names
Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
// Copy with SkipBlanks = true (default)
destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
Console.WriteLine("Results with SkipBlanks=true:");
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
}
// Reset destination values
destSheet.Cells["A1"].PutValue("Existing 1");
destSheet.Cells["A2"].PutValue("Existing 2");
destSheet.Cells["A3"].PutValue("Existing 3");
destSheet.Cells["A4"].PutValue("Existing 4");
// Copy with SkipBlanks = false
destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false });
Console.WriteLine("\nResults with SkipBlanks=false:");
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
}
}
}
}
```
### See Also
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
