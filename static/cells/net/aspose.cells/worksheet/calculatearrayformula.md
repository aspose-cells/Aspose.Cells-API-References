##Worksheet.CalculateArrayFormula
Worksheet method. Calculates a formula as array formula
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}
Calculates a formula as array formula.
```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["B3"].PutValue(6);
// Define an array formula
string arrayFormula = "=SUM(A1:B3)";
// Calculate the array formula with calculation options
object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
// Output the result
Console.WriteLine("Result of array formula calculation: " + result[0][0]);
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}
Calculates a formula as array formula.
```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount,
int maxColumnCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
| maxRowCount | Int32 | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
### Return Value
Calculated formula result.
### Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
{
public static void Run()
{
// Create a workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Example 1: Simple array formula calculation
string formula = "=ISBLANK(IF(TRUE,B2:B5))";
CalculationOptions options = new CalculationOptions();
object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);
// Example 2: Array formula with dynamic range
formula = "=LEN(IF({1;2;3;4},B2:B5))";
result = sheet.CalculateArrayFormula(formula, options, 1, 1);
Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);
// Example 3: Array formula with MATCH function
// Set up some test data
sheet.Cells["B2"].PutValue(5);
sheet.Cells["B3"].PutValue(10);
sheet.Cells["C2"].PutValue(1);
sheet.Cells["C3"].PutValue(2);
sheet.Cells["D2"].PutValue(0);
sheet.Cells["D3"].PutValue(0);
formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
result = sheet.CalculateArrayFormula(formula, options, 1, 1);
Console.WriteLine("Result of MATCH formula: " + result[0][0]);
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}
Calculates a formula as array formula.
```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts,
CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount,
int maxColumnCount, CalculationData calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula |
| cOpts | CalculationOptions | Options for calculating formula |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |
| maxRowCount | Int32 | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for [`Calculate`](../../abstractcalculationengine/calculate/). |
### Return Value
Calculated formula result.
### Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
