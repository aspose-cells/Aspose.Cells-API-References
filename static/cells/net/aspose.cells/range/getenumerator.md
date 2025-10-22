##Range.GetEnumerator
Range method. Gets the enumerator for cells in this Range
## Range.GetEnumerator method
Gets the enumerator for cells in this Range.
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
The cells enumerator
### Remarks
When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodGetEnumeratorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["B3"].PutValue("Banana");
worksheet.Cells["C2"].PutValue("Cherry");
worksheet.Cells["C3"].PutValue("Date");
// Get range and enumerate through cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
IEnumerator enumerator = range.GetEnumerator();
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
Console.WriteLine($"{cell.Name}: {cell.Value}");
}
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
