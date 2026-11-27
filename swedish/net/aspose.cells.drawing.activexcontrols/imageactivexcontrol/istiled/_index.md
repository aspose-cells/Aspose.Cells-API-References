---
title: "ImageActiveXControl.IsTiled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl egenskap. Anger om bilden är kaklad över bakgrunden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Anger om bilden är upprepad över bakgrunden.

```csharp
public bool IsTiled { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsTiledDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Image ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Ställ in IsTiled‑egenskapen och andra egenskaper
            imageControl.IsTiled = true;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;

            // Läs in en bild från fil (ersätt med din egen bildsökväg)
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            // Spara arbetsboken
            workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");

            Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
        }
    }
}
```

### Se även

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


