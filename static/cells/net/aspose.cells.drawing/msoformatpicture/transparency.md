##MsoFormatPicture.Transparency
MsoFormatPicture property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## MsoFormatPicture.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoFormatPicturePropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two pictures to the worksheet
int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
int index2 = worksheet.Pictures.Add(2, 0, "image2.png");
// Set transparency for the pictures
worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;
// Save and reload the workbook to verify the transparency settings
string outputPath = "output.xlsx";
workbook.Save(outputPath);
Workbook loadedWorkbook = new Workbook(outputPath);
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Output transparency values to console
Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
}
}
}
```
### See Also
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
