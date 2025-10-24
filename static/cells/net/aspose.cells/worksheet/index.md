##Worksheet.Index
Worksheet property. Gets the index of sheet in the worksheet collection
## Worksheet.Index property
Gets the index of sheet in the worksheet collection.
```csharp
public int Index { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add three worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Access worksheets by index and demonstrate Index property
Console.WriteLine("Worksheet Index Demonstration:");
for (int i = 0; i < workbook.Worksheets.Count; i++)
{
Worksheet sheet = workbook.Worksheets[i];
Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
}
// Add some conditional formatting to demonstrate index usage
Worksheet firstSheet = workbook.Worksheets[0];
int formatIndex = firstSheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
// Display conditional formatting index information
Console.WriteLine("\nConditional Formatting Indexes:");
Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
Console.WriteLine($"Formatting Collection Index: {formatIndex}");
Console.WriteLine($"First Condition Index: 0");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
