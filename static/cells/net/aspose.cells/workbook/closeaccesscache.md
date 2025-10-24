##Workbook.CloseAccessCache
Workbook method. Closes the session that uses caches to access data
## Workbook.CloseAccessCache method
Closes the session that uses caches to access data.
```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data and conditional formatting
for (int i = 0; i < 10; i++)
{
cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
}
// Add conditional formatting
int ruleIdx = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
Style style = workbook.CreateStyle();
style.Font.Size = 16;
fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
fcc[0].Style = style;
// Start access cache for conditional formatting
workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
// Access cells with cached conditional formatting
for (int i = 0; i < 10; i++)
{
Cell cell = cells[i, 0];
Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
}
// Close the access cache
workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
