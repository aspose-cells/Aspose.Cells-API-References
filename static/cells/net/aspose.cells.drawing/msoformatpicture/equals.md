##MsoFormatPicture.Equals
MsoFormatPicture method.
## MsoFormatPicture.Equals method
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class MsoFormatPictureMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two pictures to the worksheet
int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
Picture picture1 = worksheet.Pictures[pictureIndex1];
Picture picture2 = worksheet.Pictures[pictureIndex2];
// Get the MsoFormatPicture objects
MsoFormatPicture format1 = picture1.FormatPicture;
MsoFormatPicture format2 = picture2.FormatPicture;
// Set different properties to demonstrate equality comparison
format1.Brightness = 0.5;
format1.Contrast = 0.3;
format2.Brightness = 0.5;
format2.Contrast = 0.3;
try
{
// Compare the two MsoFormatPicture objects
bool areEqual = format1.Equals((object)format2);
Console.WriteLine($"Format objects are equal: {areEqual}");
// Modify one format and compare again
format2.Brightness = 0.7;
areEqual = format1.Equals((object)format2);
Console.WriteLine($"After modification, format objects are equal: {areEqual}");
// Compare with null
bool isNullEqual = format1.Equals((object)null);
Console.WriteLine($"Comparison with null: {isNullEqual}");
// Compare with different type
bool isDifferentTypeEqual = format1.Equals((object)"string");
Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
