##FormatCondition.Formula2
FormatCondition property. Gets and sets the value or expression associated with conditional formatting
## FormatCondition.Formula2 property
Gets and sets the value or expression associated with conditional formatting.
```csharp
public string Formula2 { get; set; }
```
### Remarks
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyFormula2Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add conditional formatting
ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
int index = conditionalFormattings.Add();
FormatConditionCollection formatConditions = conditionalFormattings[index];
// Define the cell range
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
// Add format condition with Formula2
formatConditions.Add(area,
FormatConditionType.CellValue,
OperatorType.Between,
"=\"abc def\"",
"=\"a\"&\"b\"");
// Get the format condition
FormatCondition formatCondition = formatConditions[0];
// Output the formulas
Console.WriteLine("Formula1: " + formatCondition.Formula1);
Console.WriteLine("Formula2: " + formatCondition.Formula2);
// Save the workbook
workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
