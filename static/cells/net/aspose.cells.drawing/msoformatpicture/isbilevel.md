##MsoFormatPicture.IsBiLevel
MsoFormatPicture property. Indicates whether this picture should display in twocolor black and white
## MsoFormatPicture.IsBiLevel property
Indicates whether this picture should display in two-color black and white.
```csharp
public bool IsBiLevel { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyIsBiLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
// Set the picture to bi-level (black and white)
picture.FormatPicture.IsBiLevel = true;
// Verify and output the IsBiLevel property value
Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
