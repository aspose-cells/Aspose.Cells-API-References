##HyperlinkCollection.RemoveAt
HyperlinkCollection method. Remove the hyperlink at the specified index in this collection
## HyperlinkCollection.RemoveAt method
Remove the hyperlink at the specified index in this collection.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The zero based index of the element. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a hyperlink to cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Verify hyperlink exists before removal
Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
// Remove the hyperlink at index 0
sheet.Hyperlinks.RemoveAt(0);
// Verify hyperlink was removed
Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
}
}
}
```
### See Also
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
