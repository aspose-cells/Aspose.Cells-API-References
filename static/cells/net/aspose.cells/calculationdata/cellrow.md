##CalculationData.CellRow
CalculationData property. Gets the row index of the cell where the function is in
## CalculationData.CellRow property
Gets the row index of the cell where the function is in.
```csharp
public int CellRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationDataPropertyCellRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Set calculation options
CalculationOptions opts = new CalculationOptions();
opts.CustomEngine = new CustomCalculationEngine();
// Calculate formulas
workbook.CalculateFormula(opts);
// Access the calculated cell and demonstrate CellRow property
Cell calculatedCell = worksheet.Cells["A3"];
Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
}
}
public class CustomCalculationEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
// Demonstrate accessing row information from calculation data
if (data != null)
{
Console.WriteLine("Current calculation is for row: " + data.CellRow);
}
}
}
}
```
### See Also
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
