##Cell.SetDynamicArrayFormula
Cell method. Sets dynamic array formula and make the formula spill into neighboring cells if possible
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options,
bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range. |
### Return Value
the range that the formula should spill into.
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set dynamic array formula in cell A1
Cell cell1 = cells["A1"];
cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);
// Set value in B2 that will affect the SEQUENCE formula
cells["B2"].PutValue(3);
// Calculate formulas and refresh dynamic arrays
wb.CalculateFormula();
wb.RefreshDynamicArrayFormulas(false);
// Output the results from the spilled range
Console.WriteLine("Dynamic array results:");
for (int i = 0; i < 3; i++)
{
Console.WriteLine(cells[0, i].Value);
}
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options,
object[][] values, bool calculateRange, bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | Boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
### Return Value
the range that the formula should spill into.
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
Cell cell = cells["A1"];
cell.PutValue(10);
cell = cells["A2"];
cell.PutValue(20);
cell = cells["B1"];
cell.PutValue(60);
cell = cells["B2"];
cell.PutValue(80);
// Get cell C1 where the dynamic array formula will be set
cell = worksheet.Cells["C1"];
// Define the dynamic array formula
string formula = "=A1:B2 * 2";
// Create formula parse options
FormulaParseOptions options = new FormulaParseOptions
{
Parse = true // Enable formula parsing
};
// Prepare values to populate the formula result cells
object[][] values = new object[2][];
values[0] = new object[] { 2, 4 };
values[1] = new object[] { 6, 8 };
try
{
// Set dynamic array formula with pre-calculated values
CellArea result = cell.SetDynamicArrayFormula(
formula,
options,
values,
calculateRange: false,  // Use values array dimensions for spill range
calculateValue: false  // Use provided values instead of calculating
);
Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
}
// Save the workbook with the changes
workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options,
object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | Boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | CalculationOptions | The options for calculating formula. Commonly, for performance consideration, the [`Recursive`](../../calculationoptions/recursive/) property should be false. |
### Return Value
the range that the formula should spill into.
### Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data in cells A2:B5
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(60);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["B3"].PutValue(55);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["A5"].PutValue(40);
worksheet.Cells["B5"].PutValue(70);
// Get target cell D1
Cell cellD1 = worksheet.Cells["D1"];
try
{
// Prepare parameters for SetDynamicArrayFormula
string formula = "=FILTER(A2:A5, B2:B5>50)";
FormulaParseOptions options = new FormulaParseOptions { Parse = true };
object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
bool calculateRange = true;
bool calculateValue = true;
CalculationOptions calcOptions = new CalculationOptions { Recursive = true };
// Call SetDynamicArrayFormula with specific parameters
CellArea spillRange = cellD1.SetDynamicArrayFormula(
formula,
options,
values,
calculateRange,
calculateValue,
calcOptions
);
Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
}
// Save the result
workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
