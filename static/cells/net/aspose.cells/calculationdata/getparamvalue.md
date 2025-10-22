##CalculationData.GetParamValue
CalculationData method. Gets the represented value object of the parameter at given index
## CalculationData.GetParamValue method
Gets the represented value object of the parameter at given index.
```csharp
public object GetParamValue(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the parameter(0 based) |
### Return Value
The calculated value of the parameter.
### Remarks
For one parameter:
If it is plain value, then returns the plain value itself;
If it is reference, then returns ReferredArea object;
If it references to dataset(s) with multiple values, then returns array of objects;
If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) or [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationDataMethodGetParamValueWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";
CalculationOptions options = new CalculationOptions();
options.CustomEngine = new HyperlinkCalculationEngine();
workbook.CalculateFormula(options);
}
class HyperlinkCalculationEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
{
Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
Console.WriteLine("Display Text: " + data.GetParamValue(1));
}
}
}
}
}
```
### See Also
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
