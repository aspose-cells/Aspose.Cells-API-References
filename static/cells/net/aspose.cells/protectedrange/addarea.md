##ProtectedRange.AddArea
ProtectedRange method. Adds a referred area to this
## ProtectedRange.AddArea method
Adds a referred area to this
```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column. |
| endRow | Int32 | The end row. |
| endColumn | Int32 | The end column. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add returns index of the new ProtectedRange in the collection
int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];
try
{
protectedRange.AddArea(2, 2, 5, 5);
Console.WriteLine("Added new area to protected range.");
CellArea[] areas = protectedRange.GetAreas();
Console.WriteLine($"Total protected areas: {areas.Length}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
worksheet.Protect(ProtectionType.All, "password123", null);
workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
}
}
}
```
### See Also
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
