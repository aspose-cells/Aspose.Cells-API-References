##Cell.FloatValue
Cell property. Gets the float value contained in the cell
## Cell.FloatValue property
Gets the float value contained in the cell.
```csharp
public float FloatValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyFloatValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set numeric value directly
worksheet.Cells["A1"].PutValue(3.14f);
Console.WriteLine("FloatValue of A1: " + worksheet.Cells["A1"].FloatValue);
// Set formula that returns float
worksheet.Cells["A2"].Formula = "=3.5*2";
workbook.CalculateFormula();
Console.WriteLine("FloatValue of A2: " + worksheet.Cells["A2"].FloatValue);
// Demonstrate FloatValue with shared formula
worksheet.Cells["B1"].Formula = "=5-2";
workbook.CalculateFormula();
worksheet.Cells["B1"].SetSharedFormula("=5-2", 3, 1);
workbook.CalculateFormula();
Console.WriteLine("FloatValue of B3: " + worksheet.Cells["B3"].FloatValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
