##FormatConditionCollection.GetCellArea
FormatConditionCollection method. Gets the conditional formatted cell range by index
## FormatConditionCollection.GetCellArea method
Gets the conditional formatted cell range by index.
```csharp
public CellArea GetCellArea(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the conditional formatted cell range. |
### Return Value
the conditional formatted cell range
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].Value = i + j;
}
}
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
// Set the conditional format range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 7;
area.EndColumn = 3;
fcc.AddArea(area);
// Add condition and set style
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.Yellow;
fcc[conditionIndex].Style = style;
// Get and display the cell area information
CellArea retrievedArea = fcc.GetCellArea(0);
Console.WriteLine("Conditional Format Area:");
Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
