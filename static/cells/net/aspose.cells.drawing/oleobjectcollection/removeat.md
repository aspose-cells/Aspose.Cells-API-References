##OleObjectCollection.RemoveAt
OleObjectCollection method. Removes the element at the specified index
## OleObjectCollection.RemoveAt method
Removes the element at the specified index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The specified index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OleObjectCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample OLE objects (3 objects)
for (int i = 0; i < 3; i++)
{
sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
}
Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
// Remove OLE objects one by one using RemoveAt(int index)
for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
{
sheet.OleObjects.RemoveAt(i);
}
Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
}
}
}
```
### See Also
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
