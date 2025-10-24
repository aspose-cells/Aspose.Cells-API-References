##Cells.GetEnumerator
Cells method. Gets the cells enumerator
## Cells.GetEnumerator method
Gets the cells enumerator.
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
public class CellsMethodGetEnumeratorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue(123);
worksheet.Cells["A2"].PutValue(DateTime.Now);
// Get enumerator and iterate through cells
IEnumerator enumerator = worksheet.Cells.GetEnumerator();
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
if (cell.Value != null)
{
Console.WriteLine($"{cell.Name}: {cell.Value}");
}
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
