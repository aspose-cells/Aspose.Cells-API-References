---
title: "ImageActiveXControl.PictureAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Hämtar och sätter bildens justering inom Form eller Image"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/
---
## ImageActiveXControl.PictureAlignment property

Hämtar och anger bildens justering inom formuläret eller bilden.

```csharp
public ControlPictureAlignmentType PictureAlignment { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Ställ in PictureAlignment-egenskapen
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;

            // Läs in exempelbild (ersätt med den faktiska bildsökvägen)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            workbook.Save("ImageActiveXControlDemo.xlsx");

            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
        }
    }
}
```

### Se även

* enum [ControlPictureAlignmentType](../../controlpicturealignmenttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


