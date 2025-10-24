##OleObject.ImageType
OleObject property. Gets the image format of the ole object
## OleObject.ImageType property
Gets the image format of the ole object.
```csharp
public ImageType ImageType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class OleObjectPropertyImageTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object to the worksheet
byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
// Display the current image type of the OLE object
Console.WriteLine("Current ImageType value: " + oleObject.ImageType);
// Demonstrate how to use the ImageType property
if (oleObject.ImageType == ImageType.Unknown)
{
Console.WriteLine("The OLE object's image format is not recognized.");
}
else if (oleObject.ImageType == ImageType.Emf)
{
Console.WriteLine("The OLE object uses EMF image format.");
}
else if (oleObject.ImageType == ImageType.Png)
{
Console.WriteLine("The OLE object uses PNG image format.");
}
// Save the workbook
workbook.Save("OleObjectImageTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
