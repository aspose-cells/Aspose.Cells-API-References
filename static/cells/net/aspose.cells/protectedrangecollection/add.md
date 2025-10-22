##ProtectedRangeCollection.Add
ProtectedRangeCollection method. Adds a ProtectedRange item to the collection
## ProtectedRangeCollection.Add method
Adds a [`ProtectedRange`](../../protectedrange/) item to the collection.
```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Range title. This is used as a descriptor, not as a named range definition. |
| startRow | Int32 | Start row index of the range. |
| startColumn | Int32 | Start column index of the range. |
| endRow | Int32 | End row index of the range. |
| endColumn | Int32 | End column index of the range. |
### Return Value
object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
// Add protected range with name and coordinates
int index = pranges.Add("Range1", 0, 0, 10, 10);
// Access the added range
ProtectedRange range = pranges[index];
// Set security descriptor
string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
range.SecurityDescriptor = securityDescriptor;
// Save and verify
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
