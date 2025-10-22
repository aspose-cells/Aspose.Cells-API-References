##ConditionalFormattingCollection.Copy
ConditionalFormattingCollection method. Copies conditional formatting
## ConditionalFormattingCollection.Copy method
Copies conditional formatting.
```csharp
public void Copy(ConditionalFormattingCollection cfs)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | The conditional formatting |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
{
public static void Run()
{
// Create a new workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Create a source workbook with conditional formatting
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Add sample conditional formatting to source sheet
int index = sourceSheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
// Create and apply style to the format condition
Style style = sourceWorkbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.Red;
FormatCondition fc = fcc[0];
fc.Style = style;
// Apply to a range
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 5;
area.StartColumn = 0;
area.EndColumn = 5;
fcc.AddArea(area);
// Copy conditional formatting from source to destination
destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);
// Save the workbook
destWorkbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
