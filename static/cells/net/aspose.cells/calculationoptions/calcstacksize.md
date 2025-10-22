##CalculationOptions.CalcStackSize
CalculationOptions property. The stack size for calculating cells recursively. Default value is 200
## CalculationOptions.CalcStackSize property
The stack size for calculating cells recursively. Default value is 200.
```csharp
public int CalcStackSize { get; set; }
```
### Remarks
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyCalcStackSizeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Setup sample formulas that would require stack calculation
cells["A1"].PutValue(1);
int last = 100;
cells["B1"].Formula = "=SUM(A1:A" + last + ")";
for (int i = 2; i <= last; i++)
{
cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
}
// Calculate with custom stack size
wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
Console.WriteLine("Calculation completed with custom stack size");
}
}
}
```
### See Also
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
