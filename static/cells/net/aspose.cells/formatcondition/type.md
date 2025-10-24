##FormatCondition.Type
FormatCondition property. Gets and sets whether the conditional format Type
## FormatCondition.Type property
Gets and sets whether the conditional format Type.
```csharp
public FormatConditionType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyTypeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
// Create conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Add format condition with expression type (corrected parameters)
int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
FormatCondition fc = fcs[conditionIndex];
// Set style for the condition
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
fc.Style = style;
// Demonstrate Type property usage
Console.WriteLine("Format Condition Type: " + fc.Type);
// Save the workbook
workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
