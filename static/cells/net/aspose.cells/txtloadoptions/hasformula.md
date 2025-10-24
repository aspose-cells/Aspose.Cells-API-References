##TxtLoadOptions.HasFormula
TxtLoadOptions property. Indicates whether the text is formula if it starts with
## TxtLoadOptions.HasFormula property
Indicates whether the text is formula if it starts with "=".
```csharp
public bool HasFormula { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyHasFormulaDemo
{
public static void Run()
{
// Create text load options and enable formula parsing
TxtLoadOptions options = new TxtLoadOptions();
options.HasFormula = true;
options.SeparatorString = "|";
// Load workbook with formulas in the text file
Workbook workbook = new Workbook("example.csv", options);
// Access a cell with formula and display it
Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
// Save the workbook
workbook.Save("example_output.xlsx");
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
