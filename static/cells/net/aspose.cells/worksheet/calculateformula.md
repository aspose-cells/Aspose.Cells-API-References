##Worksheet.CalculateFormula
Worksheet method. Calculates a formula
## CalculateFormula(string) {#calculateformula}
Calculates a formula.
```csharp
public object CalculateFormula(string formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
### Return Value
Calculated formula result.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateFormulaWithStringDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Settings.Region = CountryCode.USA;
Worksheet sheet = wb.Worksheets[0];
// Demonstrate basic number conversion
string formula = "=NUMBERVALUE(\"1.234\")";
Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));
// Demonstrate currency conversion
formula = "=NUMBERVALUE(\"$1,234.56\")";
Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));
// Demonstrate time conversion
formula = "=NUMBERVALUE(\"0:25\")";
Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));
// Demonstrate date conversion
formula = "=NUMBERVALUE(\"07/26/2023\")";
Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));
// Demonstrate error case
formula = "=NUMBERVALUE(\"invalid\")";
Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateFormula(string, CalculationOptions) {#calculateformula_1}
Calculates a formula expression directly.
```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
### Return Value
Calculated result of given formula. The returned object may be of possible types of [`Value`](../../cell/value/), or ReferredArea.
### Remarks
The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [`CalculateArrayFormula`](../calculatearrayformula/) instead.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Create a custom calculation engine
CustomEngine customEngine = new CustomEngine();
// Calculate formula using custom engine
CalculationOptions options = new CalculationOptions
{
CustomEngine = customEngine
};
object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
Console.WriteLine("Calculation result: " + result);
}
}
public class CustomEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "SUM")
{
double sum = 0;
for (int i = 0; i < data.ParamCount; i++)
{
object value = data.GetParamValue(i);
if (value is double)
{
sum += (double)value;
}
}
data.CalculatedValue = sum;
}
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}
Calculates a formula expression directly.
```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts,
int baseCellRow, int baseCellColumn, CalculationData calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula. |
| cOpts | CalculationOptions | Options for calculating formula. |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for [`Calculate`](../../abstractcalculationengine/calculate/). |
### Return Value
Calculated result of given formula. The returned object may be of possible types of [`Value`](../../cell/value/), or ReferredArea.
### Remarks
The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [`CalculateArrayFormula`](../calculatearrayformula/) instead.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
worksheet.Cells["B1"].PutValue(5);
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["C1"].PutValue(2);
worksheet.Cells["C2"].PutValue(4);
// Define calculation options
CalculationOptions calculationOptions = new CalculationOptions();
// Define formula parse options
FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
// Calculate formula with all parameters
object result = worksheet.CalculateFormula(
"=SUM(B1:B2, C1:C2)",  // formula
formulaParseOptions,   // parse options
calculationOptions,    // calculation options
0,                     // base cell row
0,                     // base cell column
null                   // calculation data
);
// Output the result
Console.WriteLine("Calculation result: " + result);
}
}
}
```
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}
Calculates all formulas in this worksheet.
```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
| recursive | Boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and formulas
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
// Create calculation options
CalculationOptions options = new CalculationOptions();
options.Recursive = true;
options.IgnoreError = false;
// Calculate formula with options and force full calculation
worksheet.CalculateFormula(options, true);
// Output the calculated result
Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
}
}
}
```
### See Also
* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
