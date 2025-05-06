---
title: ImageActiveXControl.Picture
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Gets and sets the data of the picture
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Gets and sets the data of the picture.

```csharp
public byte[] Picture { get; set; }
```

### Examples

```csharp
// Called: imageControl.Picture = imageData;
public static void Property_Picture()
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
            byte[] imageData = File.ReadAllBytes(&quot;ImageActiveXControlDemo.jpg&quot;);
            imageControl.Picture = imageData;

            // Save the workbook
            workbook.Save(&quot;ImageActiveXControlDemo.xlsx&quot;);
            workbook.Save(&quot;ImageActiveXControlDemo.pdf&quot;);

            // Output the results
            Console.WriteLine(&quot;Image ActiveX Control added with the following properties:&quot;);
            Console.WriteLine($&quot;IsAutoSize: {imageControl.IsAutoSize}&quot;);
            Console.WriteLine($&quot;BorderOleColor: {imageControl.BorderOleColor}&quot;);
            Console.WriteLine($&quot;BorderStyle: {imageControl.BorderStyle}&quot;);
            Console.WriteLine($&quot;PictureSizeMode: {imageControl.PictureSizeMode}&quot;);
            Console.WriteLine($&quot;SpecialEffect: {imageControl.SpecialEffect}&quot;);
            Console.WriteLine($&quot;PictureAlignment: {imageControl.PictureAlignment}&quot;);
            Console.WriteLine($&quot;IsTiled: {imageControl.IsTiled}&quot;);
        }
```

### See Also

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


