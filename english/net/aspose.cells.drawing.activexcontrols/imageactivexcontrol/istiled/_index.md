---
title: ImageActiveXControl.IsTiled
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Indicates whether the picture is tiled across the background
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Indicates whether the picture is tiled across the background.

```csharp
public bool IsTiled { get; set; }
```

### Examples

```csharp
// Called: imageControl.IsTiled = false;
public static void ImageActiveXControl_Property_IsTiled()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an Image ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Set properties for the Image ActiveX control
            imageControl.IsAutoSize = true;
            imageControl.BorderOleColor = 0x000000; // Black border
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Load an image from file and set it to the control
            byte[] imageData = File.ReadAllBytes("ImageActiveXControlDemo.jpg");
            imageControl.Picture = imageData;

            // Save the workbook
            workbook.Save("ImageActiveXControlDemo.xlsx");
            workbook.Save("ImageActiveXControlDemo.pdf");

            // Output the results
            Console.WriteLine("Image ActiveX Control added with the following properties:");
            Console.WriteLine($"IsAutoSize: {imageControl.IsAutoSize}");
            Console.WriteLine($"BorderOleColor: {imageControl.BorderOleColor}");
            Console.WriteLine($"BorderStyle: {imageControl.BorderStyle}");
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
            Console.WriteLine($"SpecialEffect: {imageControl.SpecialEffect}");
            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
            Console.WriteLine($"IsTiled: {imageControl.IsTiled}");
        }
```

### See Also

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


