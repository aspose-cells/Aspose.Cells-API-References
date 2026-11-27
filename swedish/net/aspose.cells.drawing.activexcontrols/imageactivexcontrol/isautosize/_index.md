---
title: "ImageActiveXControl.IsAutoSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Anger om kontrollen automatiskt kommer att ändra storlek för att visa hela innehållet.

```csharp
public override bool IsAutoSize { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ImageActiveXControl i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5,  // left
                5,  // top
                100, // width
                100, // height
                0,   // imageWidth (0 for default)
                0    // imageHeight (0 for default)
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Ställ in bilddata (se till att bildfilen finns)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Demonstrera IsAutoSize-egenskap
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // Spara arbetsboken
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


