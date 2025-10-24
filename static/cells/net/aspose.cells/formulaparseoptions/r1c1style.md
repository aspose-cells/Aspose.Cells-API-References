##FormulaParseOptions.R1C1Style
FormulaParseOptions property. Whether the formula is R1C1 reference style. Default is false
## FormulaParseOptions.R1C1Style property
Whether the formula is R1C1 reference style. Default is false.
```csharp
public bool R1C1Style { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaParseOptionsPropertyR1C1StyleDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
Cells cells = ws.Cells;
// Set values for referenced cells
cells["D7"].PutValue(10);
cells["D8"].PutValue(20);
cells["D9"].PutValue(30);
cells["C7"].PutValue(1);
cells["C8"].PutValue(2);
cells["C9"].PutValue(3);
// Set array formula using R1C1 style
cells[7, 4].SetArrayFormula("=TREND(RC[-1]:R[2]C[-1],RC[-2]:R[2]C[-2])", 3, 1,
new FormulaParseOptions() { R1C1Style = true });
// Output the R1C1 formulas
for (int i = 7; i < 10; i++)
{
Console.WriteLine($"Cell E{i + 1} R1C1 formula: {cells[i, 4].R1C1Formula}");
}
}
}
}
```
### See Also
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
