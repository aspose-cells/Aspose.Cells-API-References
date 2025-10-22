##Picture.DisplayAsIcon
Picture property. True if the specified object is displayed as an icon and the image will not be auto changed
## Picture.DisplayAsIcon property
True if the specified object is displayed as an icon and the image will not be auto changed.
```csharp
public bool DisplayAsIcon { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyDisplayAsIconDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
Picture picture = worksheet.Pictures[pictureIndex];
// Set DisplayAsIcon property to true
picture.DisplayAsIcon = true;
// Set other picture properties
picture.Name = "IconDisplay";
picture.Height = 100;
picture.Width = 100;
// Save the workbook
workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with icon display picture.");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
