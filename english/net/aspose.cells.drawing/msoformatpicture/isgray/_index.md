---
title: MsoFormatPicture.IsGray
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Indicates whether this picture should display in grayscale
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Indicates whether this picture should display in grayscale.

```csharp
public bool IsGray { get; set; }
```

### Examples

```csharp
// Called: formatPicture.IsGray = false;
public static void Property_IsGray()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add a picture to the worksheet
            int pictureIndex = sheet.Pictures.Add(5, 5, &quot;MsoFormatPictureDemo.jpg&quot;);
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
            workbook.Save(&quot;MsoFormatPictureDemo.xlsx&quot;);
        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


