##LoadOptions.ParsingFormulaOnOpen
LoadOptions property. Indicates whether parsing the formula when reading the file
## LoadOptions.ParsingFormulaOnOpen property
Indicates whether parsing the formula when reading the file.
```csharp
public bool ParsingFormulaOnOpen { get; set; }
```
### Remarks
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyParsingFormulaOnOpenDemo
{
public static void Run()
{
// Create load options
LoadOptions loadOptions = new LoadOptions();
// Set ParsingFormulaOnOpen to false to skip formula parsing during load
loadOptions.ParsingFormulaOnOpen = false;
// Load the workbook with the specified options
Workbook workbook = new Workbook("example.xlsm", loadOptions);
// Access worksheet and demonstrate formula parsing was skipped
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
Console.WriteLine("Cell A1 formula: " + cell.Formula);
Console.WriteLine("Cell A1 value: " + cell.Value);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
