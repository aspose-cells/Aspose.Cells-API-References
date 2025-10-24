##Class PictureBulletValue
Aspose.Cells.Drawing.Texts.PictureBulletValue class. Represents the value of the image bullet
## PictureBulletValue class
Represents the value of the image bullet.
```csharp
public class PictureBulletValue : BulletValue
```
## Constructors
| Name | Description |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Gets and sets image data of the bullet. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Gets the type of the bullet's value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
using System.IO;
public class TextsClassPictureBulletValueDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create an instance of the PictureBulletValue class
PictureBulletValue bulletValue = new PictureBulletValue();
// Load sample image data (replace with actual image path)
string imagePath = "sample.png";
if (File.Exists(imagePath))
{
bulletValue.ImageData = File.ReadAllBytes(imagePath);
// Display basic information
Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
}
else
{
Console.WriteLine("Sample image not found, using empty bullet value");
}
// Save the workbook
workbook.Save("PictureBulletValueDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
}
}
}
}
```
### See Also
* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
