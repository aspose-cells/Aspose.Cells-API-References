##CellsHelper.AddAddInFunction
CellsHelper method. Add addin function
## CellsHelper.AddAddInFunction method
Add addin function.
```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters,
int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| function | String | The function name. |
| minCountOfParameters | Int32 | Minimum number of parameters this function requires |
| maxCountOfParameters | Int32 | Maximum number of parameters this function allows. |
| paramersType | ParameterType[] | The excepted parameters type of the function |
| functionValueType | ParameterType | The function value type. |
### Remarks
NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() methods. This method will be removed 12 months later since January 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Define parameters for AddAddInFunction
string functionName = "CUSTOMFUNCTION";
int minParams = 2;
int maxParams = 4;
ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
ParameterType returnType = ParameterType.Value;
// Call the AddAddInFunction method
CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);
// Use the custom function in a cell
worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
worksheet.Cells["B2"].Value = 10;
// Calculate formulas
workbook.CalculateFormula();
Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
}
// Save the result
workbook.Save("AddAddInFunctionDemo.xlsx");
}
}
}
```
### See Also
* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
