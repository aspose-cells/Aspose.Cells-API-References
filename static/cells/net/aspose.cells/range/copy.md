##Range.Copy
Range method. Copying the range with paste special options
## Copy(Range, PasteOptions) {#copy_1}
Copying the range with paste special options.
```csharp
public void Copy(Range range, PasteOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The source range. |
| options | PasteOptions | The paste special options. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodCopyWithRangePasteOptionsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create sample data in source range
for (int i = 0; i < 5; i++)
{
for (int j = 0; j < 5; j++)
{
sheet.Cells[i, j].PutValue($"Data {i},{j}");
}
}
// Create ranges with fully qualified type
Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);
// Set paste options
PasteOptions options = new PasteOptions();
options.PasteType = PasteType.All;
// Copy with paste options
destination.Copy(source, options);
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Copy(Range) {#copy}
Copies data (including formulas), formatting, drawing objects etc. from a source range.
```csharp
public void Copy(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodCopyWithRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create source and destination ranges
Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
// Fill source range with sample data
for (int i = 0; i < 5; i++)
{
sourceRange[i, 0].PutValue($"Data {i + 1}");
}
// Copy source range to destination
sourceRange.Copy(destRange);
workbook.Save("RangeCopyDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
