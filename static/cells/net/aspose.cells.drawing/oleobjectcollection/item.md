##OleObjectCollection.Item
OleObjectCollection property. Gets the OleObject element at the specified index
## OleObjectCollection indexer
Gets the [`OleObject`](../../oleobject/) element at the specified index.
```csharp
public OleObject this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample image data
byte[] binaryImg = File.ReadAllBytes("image1.png");
// Add OLE object to the first worksheet
int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
// Access the OLE object using Item property
OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
// Set embedded object properties
byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the saved file
Workbook savedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
}
}
}
```
### See Also
* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
