##CustomFunctionDefinition.GetArrayModeParameters
CustomFunctionDefinition method. Gets the indices of given custom functions parameters that need to be calculated in array mode
## CustomFunctionDefinition.GetArrayModeParameters method
Gets the indices of given custom function's parameters that need to be calculated in array mode.
```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | String | Name of the custom function. |
### Return Value
Indices of the parameters that need to be calculated in array mode for given custom function. Default is null, there is no parameter which needs to be calculated in array mode for the custom function.
### Remarks
For an expression that needs to be calculated, taking A:A+B:B as an example: Generally in value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used for the calculation.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of CustomFunctionDefinition
CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
try
{
// Call GetArrayModeParameters with a function name parameter
string functionName = "SUM";
int[] result = customFunction.GetArrayModeParameters(functionName);
// Display the result
if (result != null)
{
Console.WriteLine("Array mode parameters for function '{0}':", functionName);
foreach (int param in result)
{
Console.WriteLine(param);
}
}
else
{
Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
}
// Save the workbook
workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
}
}
}
```
### See Also
* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
