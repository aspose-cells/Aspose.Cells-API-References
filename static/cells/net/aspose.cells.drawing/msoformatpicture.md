##Class MsoFormatPicture
Aspose.Cells.Drawing.MsoFormatPicture class. Represents the picture format
## MsoFormatPicture class
Represents the picture format.
```csharp
public class MsoFormatPicture
```
## Properties
| Name | Description |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Represents the location of the bottom of the crop rectangle expressed, in unit of inches. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Represents the brightness modification for the picture in unit of percentage. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Represents the contrast modification for the picture.in unit of percentage. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Represents gamma of the picture. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Indicates whether this picture should display in two-color black and white. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Indicates whether this picture should display in grayscale. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Represents the location of the left of the crop rectangle expressed, in unit of inches. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Represents the location of the right of the crop rectangle expressed, in unit of inches. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Represents the location of the top of the crop rectangle expressed, in unit of inches. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Gets and sets the transparent color of the picture. |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Gets the hash code. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFormatPictureDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
Picture picture = sheet.Pictures[pictureIndex];
// Access the MsoFormatPicture object
MsoFormatPicture formatPicture = picture.FormatPicture;
// Set properties of MsoFormatPicture
formatPicture.TopCropInch = 0.5;
formatPicture.BottomCropInch = 0.5;
formatPicture.LeftCropInch = 0.5;
formatPicture.RightCropInch = 0.5;
formatPicture.Transparency = 0.5;
formatPicture.Contrast = 0.8;
formatPicture.Brightness = 0.6;
formatPicture.Gamma = 1.0;
formatPicture.IsBiLevel = false;
formatPicture.IsGray = false;
// Set the transparent color
CellsColor transparentColor = workbook.CreateCellsColor();
transparentColor.Color = Color.White;
formatPicture.TransparentColor = transparentColor;
// Save the workbook
workbook.Save("MsoFormatPictureDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
