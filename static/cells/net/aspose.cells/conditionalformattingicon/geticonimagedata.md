##ConditionalFormattingIcon.GetIconImageData
ConditionalFormattingIcon method. Get the icon set data
## ConditionalFormattingIcon.GetIconImageData method
Get the icon set data
```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | IconSetType | icon's type |
| index | Int32 | icon's index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// No need to create instance since GetIconImageData is static
try
{
// Call GetIconImageData with IconSetType.Arrows3 and index 0
byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
// Save the image data to a file for demonstration
File.WriteAllBytes("icon_image.png", imageData);
Console.WriteLine("Icon image saved to icon_image.png");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
}
// Save the workbook
workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
}
}
}
```
### See Also
* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
