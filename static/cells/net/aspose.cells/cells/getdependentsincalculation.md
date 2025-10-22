##Cells.GetDependentsInCalculation
Cells method. Gets all cells whose calculated result depends on specific cell
## Cells.GetDependentsInCalculation method
Gets all cells whose calculated result depends on specific cell.
```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index of the specific cell |
| column | Int32 | Column index of the specific cell. |
| recursive | Boolean | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |
### Return Value
Enumerator to enumerate all dependents(Cell objects)
### Remarks
To use this method, please make sure the workbook has been set with true value for [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook and calculate formulas
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set up formula dependencies:
// C1 = 10 (source value)
// B1 = C1*2
// A1 = B1+5
cells["C1"].PutValue(10);
cells["B1"].Formula = "C1*2";
cells["A1"].Formula = "B1+5";
// Calculate formulas to establish dependencies
workbook.CalculateFormula();
try
{
// Get dependents for cell C1 (row 0, column 2) with recursive check
IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);
Console.WriteLine("Dependents of cell C1:");
while (dependents.MoveNext())
{
if (dependents.Current is Cell dependentCell)
{
Console.WriteLine($"- {dependentCell.Name}");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
}
// Save the workbook
workbook.Save("GetDependentsInCalculationDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
