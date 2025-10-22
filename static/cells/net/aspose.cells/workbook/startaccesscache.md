##Workbook.StartAccessCache
Workbook method. Starts the session that uses caches to access data
## Workbook.StartAccessCache method
Starts the session that uses caches to access data.
```csharp
public void StartAccessCache(AccessCacheOptions opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options of data access |
### Remarks
If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them.  After finishing the access to the data, [`CloseAccessCache`](../closeaccesscache/) should be invoked with same options to clear all caches and recover normal access mode.
### Examples
```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add conditional formatting
ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
int index = cfc.Add();
cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
FormatConditionType.DuplicateValues, OperatorType.None, null, null);
// Set style for conditional formatting
Style style = cfc[0][0].Style;
style.ForegroundColor = Color.Red;
style.Pattern = BackgroundType.Solid;
// Add some embedded images
Cells cells = sheet.Cells;
byte[] img1 = File.ReadAllBytes("1.png");
byte[] img2 = File.ReadAllBytes("2.png");
cells[0, 0].EmbeddedImage = img1;
cells[2, 0].EmbeddedImage = img2;
cells[4, 0].EmbeddedImage = img1;
// Start access cache for better performance
wb.StartAccessCache(AccessCacheOptions.All);
// Access cell styles (will be faster due to caching)
Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
// Close the cache when done
wb.CloseAccessCache(AccessCacheOptions.All);
}
}
}
```
### See Also
* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
