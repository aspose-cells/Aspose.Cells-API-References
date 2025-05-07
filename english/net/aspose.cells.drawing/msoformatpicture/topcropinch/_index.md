---
title: MsoFormatPicture.TopCropInch
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the location of the top of the crop rectangle expressed in unit of inches
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Represents the location of the top of the crop rectangle expressed, in unit of inches.

```csharp
public double TopCropInch { get; set; }
```

### Examples

```csharp
// Called: formatPicture.TopCropInch = 0.5;
public static void Property_TopCropInch()
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
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


