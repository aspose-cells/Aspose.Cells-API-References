##CellRichValue.ErrorValue
CellRichValue property. Gets the error value type of the cell
## CellRichValue.ErrorValue property
Gets the error value type of the cell.
```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellRichValuePropertyErrorValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a spill error in cell A1
worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
try
{
// Calculate formulas to generate the spill error
workbook.CalculateFormula();
}
catch (Exception)
{
// Expected spill error
}
// Get rich value from cell A1
CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
// Check and display the error type
Console.WriteLine("Error type: " + richValue.ErrorValue);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
