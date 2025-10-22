##Workbook.RefreshDynamicArrayFormulas
Workbook method. Refreshes dynamic array formulasspill into new range of neighboring cells according to current data Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.
```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | Boolean | Whether calculates and updates cell values for those dynamic array formulas |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet1 = wb.Worksheets[0];
Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
// Set up initial data and dynamic array formulas
sheet1.Cells["A1"].PutValue("B1:B3");
sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);
Console.WriteLine("Before refresh:");
PrintSpillStatus(sheet1, sheet2);
// Change the range and refresh formulas
sheet1.Cells["A1"].PutValue("B1:B5");
wb.RefreshDynamicArrayFormulas(true);
Console.WriteLine("\nAfter refresh:");
PrintSpillStatus(sheet1, sheet2);
}
private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
{
Console.WriteLine("Sheet1 spill range:");
for (int i = 1; i <= 6; i++)
{
Cell cell = sheet1.Cells.CheckCell(i, 0);
Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
}
Console.WriteLine("\nSheet2 spill range:");
for (int i = 1; i <= 6; i++)
{
Cell cell = sheet2.Cells.CheckCell(0, i);
Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | Boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | CalculationOptions | The options for calculating formulas |
### Remarks
For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc. For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by [`CalculateFormula`](../calculateformula/)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample dynamic array formula
worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
// Create calculation options
CalculationOptions opts = new CalculationOptions();
opts.CalcStackSize = 100;
// Refresh dynamic array formulas with calculation options
workbook.RefreshDynamicArrayFormulas(true, opts);
// Calculate workbook formulas
workbook.CalculateFormula(opts);
// Output result from A1:A5
for (int i = 0; i < 5; i++)
{
Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
}
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
