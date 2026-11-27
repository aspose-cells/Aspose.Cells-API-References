---
title: "Enum ControlPictureSizeMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Representerar hur bilden ska visas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Representerar hur bilden ska visas.

```csharp
public enum ControlPictureSizeMode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Clip | `0` | Beskär alla delar av bilden som är större än kontrollens gränser. |
| Stretch | `1` | Sträcker bilden för att fylla kontrollens område. Denna inställning förvränger bilden i antingen horisontell eller vertikal riktning. |
| Zoom | `3` | Förstorar bilden, men förvränger inte bilden i någon horisontell eller vertikal riktning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i kalkylbladet
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Lägg till en ImageActiveXControl i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Ange bilddata för ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Ange PictureSizeMode till Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Ange andra egenskaper för ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Spara arbetsboken
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


