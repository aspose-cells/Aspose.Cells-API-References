##Worksheet.CloseAccessCache
Worksheet method. Closes the session that uses caches to access the data in this worksheet
## Worksheet.CloseAccessCache method
Closes the session that uses caches to access the data in this worksheet.
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
public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Populate cells with sample data
for (int i = 0; i < 1000; i++)
{
cells[i, 0].PutValue(i % 10);
}
// Add conditional formatting
FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
fcs.AddCondition(FormatConditionType.ColorScale);
// Enable access cache for conditional formatting
sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);
// Perform operations with cached access
Random random = new Random();
for (int i = 0; i < 100; i++)
{
int r = random.Next(0, 1000);
var style = cells[r, 0].GetDisplayStyle();
Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
}
// Close the access cache
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
