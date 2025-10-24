##FormatCondition.Text
FormatCondition property. The text value in a text contains conditional formatting rule. Valid only for type  containsText notContainsText beginsWith and endsWith. The default value is null
## FormatCondition.Text property
The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyTextDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add conditional formatting
ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
int collectionIndex = conditionalFormattings.Add();
FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];
// Add text condition
int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
FormatCondition formatCondition = formatConditions[conditionIndex];
// Set the text property (demonstrating Russian text)
formatCondition.Text = "вс";
// Apply formatting style
Style style = formatCondition.Style;
style.BackgroundColor = Color.Red;
formatCondition.Style = style;
// Apply to cell A1
formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));
// Save and verify
string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
workbook.Save(outputPath);
Console.WriteLine("FormatCondition Text property demo completed successfully.");
}
}
}
```
### See Also
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
