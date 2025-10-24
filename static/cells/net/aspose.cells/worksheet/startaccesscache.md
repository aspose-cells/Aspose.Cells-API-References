##Worksheet.StartAccessCache
Worksheet method. Starts the session that uses caches to access the data in this worksheet
## Worksheet.StartAccessCache method
Starts the session that uses caches to access the data in this worksheet.
```csharp
public void StartAccessCache(AccessCacheOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |
### Remarks
After finishing the access to the data, [`CloseAccessCache`](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Set default style
Style style = wb.DefaultStyle;
style.Font.Size = 10;
wb.DefaultStyle = style;
// Add conditional formatting
ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
FormatConditionCollection fcc = cfc[cfc.Add()];
fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
fcc.AddCondition(FormatConditionType.DuplicateValues);
FormatCondition fc = fcc[0];
fc.Style.Font.Size = 16;
// Populate some data
Cells cells = sheet.Cells;
for (int i = 0; i < 10; i++)
{
cells[0, i].PutValue("A");
cells[i, 0].PutValue(i);
}
// Start access cache for better performance
sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
// Verify styles
for (int i = 0; i < 10; i++)
{
Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
}
// Close cache when done
sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
}
}
}
```
### See Also
* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
