---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Hämtar och sätter hur bilden ska visas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Hämtar och anger hur bilden ska visas.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Image ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Ställ in PictureSizeMode och andra egenskaper
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Läs in en exempelbild (ersätt med din egen bildsökväg)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Spara arbetsboken
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Skriv ut värdet för PictureSizeMode
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Se även

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


