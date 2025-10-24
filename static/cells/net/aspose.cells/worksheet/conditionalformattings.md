##Worksheet.ConditionalFormattings
Worksheet property. Gets the ConditionalFormattings in the worksheet
## Worksheet.ConditionalFormattings property
Gets the ConditionalFormattings in the worksheet.
```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyConditionalFormattingsDemo
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
FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
// Set the range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 0;
fcc.AddArea(area);
// Add condition
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
FormatCondition fc = fcc[conditionIndex];
fc.Style.BackgroundColor = System.Drawing.Color.Red;
// Save the workbook
workbook.Save("ConditionalFormattingDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
