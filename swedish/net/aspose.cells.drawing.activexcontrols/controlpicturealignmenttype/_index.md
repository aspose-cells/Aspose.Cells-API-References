---
title: "Enum ControlPictureAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType enum. Representerar justeringen av bilden inuti formuläret eller bilden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Representerar justeringen av bilden inuti Form eller Image.

```csharp
public enum ControlPictureAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| TopLeft | `0` | Det övre vänstra hörnet. |
| TopRight | `1` | Det övre högra hörnet. |
| Center | `2` | Mitten. |
| BottomLeft | `3` | Det nedre vänstra hörnet. |
| BottomRight | `4` | Det nedre högra hörnet. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ImageActiveXControl med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Ställ in bildens egenskaper
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Spara arbetsboken
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


