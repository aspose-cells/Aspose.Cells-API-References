##ProtectedRangeCollection.Item
ProtectedRangeCollection property. Gets the ProtectedRange element at the specified index
## ProtectedRangeCollection indexer
Gets the [`ProtectedRange`](../../protectedrange/) element at the specified index.
```csharp
public ProtectedRange this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangeCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a protected range using cell indices (startRow, startColumn, endRow, endColumn)
int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
protectedRange.Password = "password123";
// Access the protected range using Item property (index 0)
ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
// Verify and display protection status
Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
Console.WriteLine("Range name: " + retrievedRange.Name);
// Save the workbook
workbook.Save("ProtectedRangeDemo.xlsx");
}
}
}
```
### See Also
* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
