---
title: ImageActiveXControl.IsAutoSize
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Indicates whether the control will automatically resize to display its entire contents
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Indicates whether the control will automatically resize to display its entire contents.

```csharp
public override bool IsAutoSize { get; set; }
```

### Examples

```csharp
// Called: imageControl.IsAutoSize = true;
public static void ImageActiveXControl_Property_IsAutoSize()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an image to the worksheet
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Add an ImageActiveXControl to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Set the picture data for the ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Set the PictureSizeMode to Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Set other properties of the ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Save the workbook
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
```

### See Also

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


