##Workbook.ParseFormulas
Workbook method. Parses all formulas which have not been parsed when they were loaded from template file or set to a cell
## Workbook.ParseFormulas method
Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.
```csharp
public void ParseFormulas(bool ignoreError)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Whether ignore error for invalid formula. For one invalid formula, if ignore error then this formula will be ignored and the process will continue to parse other formulas, otherwise exception will be thrown. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodParseFormulasWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets[0];
Cells cells = worksheet.Cells;
// Set formulas without parsing (Parse = false)
for (int i = 1; i < 10; i++)
{
cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
}
Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");
// Parse all formulas at once
wb.ParseFormulas(false);
// Verify the formulas
for (int i = 1; i < 10; i++)
{
Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
