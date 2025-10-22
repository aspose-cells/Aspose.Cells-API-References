##Workbook.UpdateCustomFunctionDefinition
Workbook method. Updates definition of custom functions
## Workbook.UpdateCustomFunctionDefinition method
Updates definition of custom functions.
```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```
| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |
### Remarks
This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data
sheet.Cells["B1"].PutValue(1);
sheet.Cells["C1"].PutValue(2);
sheet.Cells["B2"].PutValue(4);
sheet.Cells["C2"].PutValue(8);
// Create custom calculation engine
var customEngine = new MyCustomCalculationEngine();
// Set calculation options with custom engine
CalculationOptions options = new CalculationOptions
{
CustomEngine = customEngine
};
// Update the custom function definition
wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());
// Set formula using custom function
sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
// Calculate formulas
wb.CalculateFormula(options);
// Output the result
Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
}
}
public class MyCustomFunctionDefinition : CustomFunctionDefinition
{
public override int[] GetArrayModeParameters(string functionName)
{
// Return parameter indices that should be processed in array mode
return new int[] { 0 }; // First parameter is array mode
}
}
public class MyCustomCalculationEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "MYFUNC")
{
double sum = 0;
var paramValue = data.GetParamValue(0);
if (paramValue is object[,] arrayValue)
{
foreach (var val in arrayValue)
{
if (val != null)
{
sum += Convert.ToDouble(val);
}
}
}
else
{
sum += Convert.ToDouble(paramValue);
}
data.CalculatedValue = sum * 2; // Custom calculation logic
}
}
}
}
```
### See Also
* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
