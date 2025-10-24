##Name.GetRanges
Name method. Gets all ranges referred by this name
## GetRanges() {#getranges}
Gets all ranges referred by this name.
```csharp
public Range[] GetRanges()
```
### Return Value
All ranges.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameMethodGetRangesDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Cherry");
// Create a named range
int index = workbook.Worksheets.Names.Add("Fruits");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet1!$A$1:$A$3";
// Get ranges with recalculation
Aspose.Cells.Range[] ranges1 = name.GetRanges();
Console.WriteLine("Ranges with recalculation:");
PrintRanges(ranges1);
// Get ranges without recalculation
Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
Console.WriteLine("\nRanges without recalculation:");
PrintRanges(ranges2);
}
private static void PrintRanges(Aspose.Cells.Range[] ranges)
{
if (ranges != null)
{
foreach (Aspose.Cells.Range range in ranges)
{
Console.WriteLine($"Range: {range.Address}");
}
}
else
{
Console.WriteLine("No ranges found");
}
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetRanges(bool) {#getranges_1}
Gets all ranges referred by this name.
```csharp
public Range[] GetRanges(bool recalculate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |
### Return Value
All ranges.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameMethodGetRangesWithBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Test");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
// Create a named range
int index = workbook.Worksheets.Names.Add("TestRange");
Name namedRange = workbook.Worksheets.Names[index];
namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
// Get ranges without recalculating
Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
// Get ranges with recalculating
Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
// Modify the range and demonstrate recalculation
worksheet.Cells["A4"].PutValue(30);
namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
// Get ranges with and without recalculating after modification
Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
