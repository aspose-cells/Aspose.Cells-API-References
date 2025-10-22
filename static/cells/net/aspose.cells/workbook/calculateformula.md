##Workbook.CalculateFormula
Workbook method. Calculates the result of formulas
## CalculateFormula() {#calculateformula}
Calculates the result of formulas.
```csharp
public void CalculateFormula()
```
### Remarks
For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCalculateFormulaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set values and formulas
cells["A1"].PutValue(5);
cells["B1"].Formula = "=A1*2";
cells["C1"].Formula = "=B1+10";
// Calculate formulas
workbook.CalculateFormula();
// Display results
Console.WriteLine("A1 value: " + cells["A1"].IntValue);
Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateFormula(bool) {#calculateformula_2}
Calculates the result of formulas.
```csharp
public void CalculateFormula(bool ignoreError)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | Boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCalculateFormulaWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access the first worksheet and its cells
Worksheet worksheet = wb.Worksheets[0];
Cells cells = worksheet.Cells;
// Put values in the first row (A1:E1)
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue(i + 1); // Values 1-5
}
// Put values in the second row (A2:E2)
for (int i = 0; i < 5; i++)
{
cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
}
// Set a shared HLOOKUP formula in the fourth row (A4:E4)
cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);
// Calculate formulas without recursive calculation
wb.CalculateFormula(false);
// Display the results
Console.WriteLine("Formula calculation results:");
for (int i = 0; i < 5; i++)
{
Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateFormula(CalculationOptions) {#calculateformula_1}
Calculating formulas in this workbook.
```csharp
public void CalculateFormula(CalculationOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create a table and set column names
sheet.Cells["A1"].PutValue("A");
sheet.Cells["B1"].PutValue("B");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["B2"].PutValue(2);
// Set formulas and calculate
Cells cells = sheet.Cells;
cells["C1"].PutValue("InvalidColumn");
cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
// Calculate formulas with options
wb.CalculateFormula(new CalculationOptions());
// Output results
Console.WriteLine("D1 result: " + cells["D1"].StringValue);
Console.WriteLine("E1 result: " + cells["E1"].StringValue);
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
