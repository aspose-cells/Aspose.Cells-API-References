##Cells.CountLarge
Cells property. Gets the total count of instantiated Cell objects
## Cells.CountLarge property
Gets the total count of instantiated Cell objects.
```csharp
public long CountLarge { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyCountLargeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B2"].PutValue("World");
worksheet.Cells["C3"].PutValue(123);
// Demonstrate CountLarge property
long cellCount = worksheet.Cells.CountLarge;
Console.WriteLine($"Total cells in worksheet: {cellCount}");
// Show paper size for demonstration
Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
