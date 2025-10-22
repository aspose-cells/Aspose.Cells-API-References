##CalculationData.CalculatedValue
CalculationData property. Gets or sets the calculated value for this function
## CalculationData.CalculatedValue property
Gets or sets the calculated value for this function.
```csharp
public object CalculatedValue { get; set; }
```
### Remarks
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of [`Value`](../../cell/value/), or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationDataPropertyCalculatedValueDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
// Create calculation options with custom engine
CalculationOptions options = new CalculationOptions();
options.CustomEngine = new CustomCalculationEngine();
// Calculate formulas with options
workbook.CalculateFormula(options);
// Get the calculated value
Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
}
}
public class CustomCalculationEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "SUM")
{
double sum = 0;
for (int i = 0; i < data.ParamCount; i++)
{
object arg = data.GetParamValue(i);
if (arg is double)
{
sum += (double)arg;
}
}
data.CalculatedValue = sum;
}
}
}
}
```
### See Also
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
