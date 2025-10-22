##PictureBulletValue.ImageData
PictureBulletValue property. Gets and sets image data of the bullet
## PictureBulletValue.ImageData property
Gets and sets image data of the bullet.
```csharp
public byte[] ImageData { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
using System.IO;
public class PictureBulletValuePropertyImageDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create an instance of PictureBulletValue
PictureBulletValue bulletValue = new PictureBulletValue();
// Demonstrate setting and getting ImageData
byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
bulletValue.ImageData = sampleImageData;
// Display the ImageData property value
Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
// Show the Type property (read-only)
Console.WriteLine("Bullet Type: " + bulletValue.Type);
// Save the workbook
workbook.Save("PictureBulletValueImageDataDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
