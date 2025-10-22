##HorizontalPageBreakCollection.RemoveAt
HorizontalPageBreakCollection method. Removes the HPageBreak element at a specified name
## HorizontalPageBreakCollection.RemoveAt method
Removes the HPageBreak element at a specified name.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Element index, zero based. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.HorizontalPageBreaks.Add(5);
worksheet.HorizontalPageBreaks.Add(10);
worksheet.HorizontalPageBreaks.Add(15);
worksheet.HorizontalPageBreaks.RemoveAt(0);
workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
