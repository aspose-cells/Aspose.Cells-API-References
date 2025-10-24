##Class CalculationOptions
Aspose.Cells.CalculationOptions class. Represents options for calculation
## CalculationOptions class
Represents options for calculation.
```csharp
public class CalculationOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | The stack size for calculating cells recursively. Default value is 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | The monitor for user to track the progress of formula calculation. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Specifies the data sources for external links used in formulas. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Specifies the strategy for processing precision of calculation. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Text;
public class CalculationOptionsDemo
{
public static void CalculationOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(10.555);
worksheet.Cells["A2"].PutValue(20.6666);
worksheet.Cells["A3"].PutValue(30.7777);
worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";
// Create an instance of CalculationOptions
CalculationOptions calcOptions = new CalculationOptions
{
IgnoreError = true,
Recursive = true,
CalcStackSize = 200,
PrecisionStrategy = CalculationPrecisionStrategy.Round,
CharacterEncoding = Encoding.UTF8
};
// Optionally, you can set a custom calculation engine or monitor
// calcOptions.CustomEngine = new MyCustomEngine();
// calcOptions.CalculationMonitor = new MyCalculationMonitor();
// Calculate formulas in the workbook with the specified options
workbook.CalculateFormula(calcOptions);
// Save the workbook
workbook.Save("CalculationOptionsExample.xlsx");
workbook.Save("CalculationOptionsExample.pdf");
}
}
// Example custom calculation engine (if needed)
public class MyCustomEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
// Custom calculation logic
string funcName = data.FunctionName.ToUpper();
if (funcName == "MYFUNC")
{
// Example custom function logic
int count = data.ParamCount;
object result = null;
for (int i = 0; i < count; i++)
{
object paramValue = data.GetParamValue(i);
if (paramValue is ReferredArea)
{
ReferredArea ra = (ReferredArea)paramValue;
paramValue = ra.GetValue(0, 0);
}
// Process the parameter here
// result = ...;
}
data.CalculatedValue = result;
}
}
}
// Example custom calculation monitor (if needed)
public class MyCalculationMonitor : AbstractCalculationMonitor
{
public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
{
// Logic before calculation
Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
}
public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
{
// Logic after calculation
Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
}
public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
{
// Handle circular references
Console.WriteLine("Circular reference detected.");
return true; // Continue calculation
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
