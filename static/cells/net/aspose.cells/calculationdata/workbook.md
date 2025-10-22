##CalculationData.Workbook
CalculationData property. Gets the Workbook object where the function is in
## CalculationData.Workbook property
Gets the Workbook object where the function is in.
```csharp
public Workbook Workbook { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CalculationDataPropertyWorkbookDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formula
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";
// Create calculation options and register custom calculation engine
CalculationOptions options = new CalculationOptions();
options.CustomEngine = new CustomCalcEngine();
// Trigger calculation with options to demonstrate Workbook property usage
workbook.CalculateFormula(options);
// Display result from calculation
Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);
// Save the result
workbook.Save("PropertyWorkbookDemo.xlsx");
}
private class CustomCalcEngine : AbstractCalculationEngine
{
public override void Calculate(CalculationData data)
{
if (data.FunctionName == "CUSTOMFUNC")
{
// Access Workbook property from CalculationData
Workbook currentWorkbook = data.Workbook;
Worksheet currentSheet = currentWorkbook.Worksheets[0];
// Demonstrate using workbook to manipulate data
double inputValue = (double)currentSheet.Cells["A1"].Value;
currentSheet.Cells["C1"].PutValue(inputValue * 2);
// Set calculated result
data.CalculatedValue = inputValue * 3;
}
}
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
