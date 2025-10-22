##CalculationData.GetParamText
CalculationData method. Gets the literal text of the parameter at given index
## CalculationData.GetParamText method
Gets the literal text of the parameter at given index.
```csharp
public string GetParamText(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index of the parameter(0 based) |
### Return Value
literal text of the parameter
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationDataMethodGetParamTextWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].Formula = "=SUM(INDIRECT(\"'Book2.xlsx'!Table1[#All]\"))";
CalculationOptions options = new CalculationOptions();
options.CustomEngine = new CustomCalcEngine();
workbook.CalculateFormula(options);
}
}
class CustomCalcEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "SUM")
{
Console.WriteLine("SUM parameter: " + data.GetParamText(0));
}
else if (data.FunctionName == "INDIRECT")
{
Console.WriteLine("INDIRECT parameter: " + data.GetParamText(0));
}
}
}
}
```
### See Also
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
