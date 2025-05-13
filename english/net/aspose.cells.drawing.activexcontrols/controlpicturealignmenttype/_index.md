---
title: Enum ControlPictureAlignmentType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType enum. Represents the alignment of the picture inside the Form or Image
type: docs
url: /net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Represents the alignment of the picture inside the Form or Image.

```csharp
public enum ControlPictureAlignmentType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| TopLeft | `0` | The top left corner. |
| TopRight | `1` | The top right corner. |
| Center | `2` | The center. |
| BottomLeft | `3` | The bottom left corner. |
| BottomRight | `4` | The bottom right corner. |

### Examples

```csharp
// Called: imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
public static void ActiveXControls_Type_ControlPictureAlignmentType()
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

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


