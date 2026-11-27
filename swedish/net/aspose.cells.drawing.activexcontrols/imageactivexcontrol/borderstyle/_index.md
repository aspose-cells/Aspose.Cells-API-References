---
title: "ImageActiveXControl.BorderStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Hämtar och sätter typen av ram som används av kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/
---
## ImageActiveXControl.BorderStyle property

Hämtar och anger typen av ram som används av kontrollen.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5, 5, 100, 100, 200, 200);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Ställ in ramstil och demonstrera dess användning
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black border

            // Ställ in exempelbild (se till att den här filen finns i din körkatalog)
            if (File.Exists("sample.png"))
            {
                imageControl.Picture = File.ReadAllBytes("sample.png");
            }

            workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


