##Enum CalcModeType
Aspose.Cells.CalcModeType enum. Represents the mode type of calculating formulas
## CalcModeType enumeration
Represents the mode type of calculating formulas.
```csharp
public enum CalcModeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` |  |
| AutomaticExceptTable | `1` |  |
| Manual | `2` |  |
### Remarks
Only sets for MS Excel.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CalcModeTypeDemo
{
public static void CalcModeTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for test
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["B2"].PutValue(3);
worksheet.Cells["B3"].PutValue(4);
worksheet.Cells["C1"].PutValue(5);
worksheet.Cells["C2"].PutValue(10);
worksheet.Cells["C3"].PutValue(15);
worksheet.Cells["A4"].Formula = "=A1+B1+C1";
worksheet.Cells["B4"].Formula = "=SUM(B1:B3)";
// Access the formula settings of the workbook
FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;
// Set the calculation mode to Manual
formulaSettings.CalculationMode = CalcModeType.Manual;
// Set other formula settings
formulaSettings.CalculateOnOpen = true;
formulaSettings.CalculateOnSave = true;
formulaSettings.ForceFullCalculation = false;
formulaSettings.CalculationId = "0";
formulaSettings.EnableIterativeCalculation = true;
formulaSettings.MaxIteration = 100;
formulaSettings.MaxChange = 0.001;
formulaSettings.PrecisionAsDisplayed = false;
formulaSettings.EnableCalculationChain = true;
formulaSettings.PreservePaddingSpaces = false;
// Save the workbook
workbook.Save("CalcModeTypeExample.xlsx");
workbook.Save("CalcModeTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
