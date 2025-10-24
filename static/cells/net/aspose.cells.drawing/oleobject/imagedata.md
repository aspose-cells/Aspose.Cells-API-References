##OleObject.ImageData
OleObject property. Represents image of ole object as byte array
## OleObject.ImageData property
Represents image of ole object as byte array.
```csharp
public byte[] ImageData { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyImageDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Read image file into byte array
byte[] imageBytes = File.ReadAllBytes("image1.png");
// Add OLE object with the image data
int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
// Set embedded object properties
oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
// Demonstrate ImageData property usage
Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
// Save the workbook
workbook.Save("OleObjectWithImage.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
