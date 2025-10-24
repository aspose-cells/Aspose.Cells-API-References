##Cells.ImportFormulaArray
Cells method. Imports an array of formula into a worksheet
## Cells.ImportFormulaArray method
Imports an array of formula into a worksheet.
```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | String[] | Formula array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare formula array and parameters
string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
int firstRow = 0;
int firstColumn = 0;
bool isVertical = true;
try
{
// Import formulas vertically starting at cell A1
worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
// Set values for formula references
worksheet.Cells["A1"].PutValue(2);
worksheet.Cells["B1"].PutValue(3);
worksheet.Cells["C1"].PutValue(4);
worksheet.Cells["D1"].PutValue(5);
// Calculate formulas
workbook.CalculateFormula();
Console.WriteLine("Formulas imported successfully. Calculated results:");
Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
