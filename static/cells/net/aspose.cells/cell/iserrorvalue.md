##Cell.IsErrorValue
Cell property. Checks if the value of this cell is an error
## Cell.IsErrorValue property
Checks if the value of this cell is an error.
```csharp
public bool IsErrorValue { get; }
```
### Remarks
Also applies to formula cell to check whether the calculated result is an error.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsErrorValueDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set a formula that will result in an error
Cell cell = cells["A1"];
cell.Formula = "=1/0"; // Division by zero error
// Calculate formulas
workbook.CalculateFormula();
// Demonstrate IsErrorValue property
Console.WriteLine("Cell A1 value: " + cell.StringValue);
Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
Console.WriteLine("Error type: " + cell.Value);
// Set a valid value
Cell cell2 = cells["A2"];
cell2.PutValue("Valid value");
Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);
// Set a SPILL error (Excel 365+ dynamic array formula error)
Cell cell3 = cells["A3"];
cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
