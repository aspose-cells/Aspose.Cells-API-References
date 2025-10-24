##FormatCondition.Style
FormatCondition property. Gets or setts style of conditional formatted cell ranges
## FormatCondition.Style property
Gets or setts style of conditional formatted cell ranges.
```csharp
public Style Style { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyStyleDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(30);
worksheet.Cells["A2"].PutValue(60);
worksheet.Cells["A3"].PutValue(90);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the range
CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
fcs.AddArea(area);
// Add first condition (values between 40-80)
int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
FormatCondition fc1 = fcs[conditionIndex1];
fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
fc1.Style.Font.Color = System.Drawing.Color.Black;
// Add second condition (values > 80)
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
FormatCondition fc2 = fcs[conditionIndex2];
fc2.Style.BackgroundColor = System.Drawing.Color.Green;
fc2.Style.Font.Color = System.Drawing.Color.White;
fc2.Style.Font.IsBold = true;
// Save the workbook
workbook.Save("FormatConditionStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
