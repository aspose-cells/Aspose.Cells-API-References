##Cell.IsFormula
Cell property. Represents if the specified cell contains formula
## Cell.IsFormula property
Represents if the specified cell contains formula.
```csharp
public bool IsFormula { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add formula to cell A1
worksheet.Cells["A1"].Formula = "=1+2";
// Add plain value to cell A2
worksheet.Cells["A2"].PutValue("Test");
// Check if cells contain formulas
Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
