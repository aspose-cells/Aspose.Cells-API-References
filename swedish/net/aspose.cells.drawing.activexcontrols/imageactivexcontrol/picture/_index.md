---
title: "ImageActiveXControl.Picture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Hämtar och sätter bildens data"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Hämtar och anger bildens data.

```csharp
public byte[] Picture { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Image ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Ställ in Picture-egenskapen (med en exempelbild som byte-array)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Verifiera att Picture-egenskapen har satts
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Spara arbetsboken
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


