##FormatCondition.Formula1
FormatCondition property. Gets and sets the value or expression associated with conditional formatting
## FormatCondition.Formula1 property
Gets and sets the value or expression associated with conditional formatting.
```csharp
public string Formula1 { get; set; }
```
### Remarks
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyFormula1Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["E1"].PutValue(50);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Set the range and condition type
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 5;
area.EndColumn = 5;
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
// Access and display the Formula1 property
FormatCondition fc = fcc[0];
Console.WriteLine("Formula1: " + fc.Formula1);
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
