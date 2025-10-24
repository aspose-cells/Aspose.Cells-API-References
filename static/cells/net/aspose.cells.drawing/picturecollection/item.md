##PictureCollection.Item
PictureCollection property. Gets the Picture element at the specified index
## PictureCollection indexer
Gets the [`Picture`](../../picture/) element at the specified index.
```csharp
public Picture this[int index] { get; }
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
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PictureCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get picture collection
PictureCollection pictures = worksheet.Pictures;
// Add a picture (replace "image.png" with actual image path)
int index = pictures.Add(1, 1, "image.png");
// Access the picture using Item property
Picture pic = pictures[index];
// Demonstrate Item property usage
Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
// Modify picture properties
pic.Height = 200;
pic.Width = 300;
// Save the workbook
workbook.Save("PictureCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
