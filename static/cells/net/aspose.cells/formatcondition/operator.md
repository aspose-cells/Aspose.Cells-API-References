##FormatCondition.Operator
FormatCondition property. Gets and sets the conditional format operator type
## FormatCondition.Operator property
Gets and sets the conditional format operator type.
```csharp
public OperatorType Operator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyOperatorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Create cell range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 0;
// Add condition
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
FormatCondition fc = fcc[conditionIndex];
// Set style
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
fc.Style = style;
// Demonstrate Operator property usage
Console.WriteLine("Operator Type: " + fc.Operator);
if (fc.Operator == OperatorType.Between)
{
Console.WriteLine("Condition is set to BETWEEN values");
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
