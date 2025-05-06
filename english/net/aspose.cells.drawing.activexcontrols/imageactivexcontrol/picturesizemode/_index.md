---
title: ImageActiveXControl.PictureSizeMode
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Gets and sets how to display the picture
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Gets and sets how to display the picture.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Examples

```csharp
// Called: imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;
public static void Property_PictureSizeMode()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an image to the worksheet
            int pictureIndex = worksheet.Pictures.Add(1, 1, &quot;ControlPictureSizeMode.png&quot;);
            Picture picture = worksheet.Pictures[pictureIndex];

            // Add an ImageActiveXControl to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Set the picture data for the ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes(&quot;ControlPictureSizeMode.png&quot;);

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
            workbook.Save(&quot;ControlPictureSizeModeExample.xlsx&quot;);
            workbook.Save(&quot;ControlPictureSizeModeExample.pdf&quot;);
        }
```

### See Also

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


