---
title: "LabelActiveXControl.Picture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl egenskap. Hämtar och anger bildens data"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/
---
## LabelActiveXControl.Picture property

Hämtar och anger bildens data.

```csharp
public byte[] Picture { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Label ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Ställ in grundläggande egenskaper
            labelControl.Caption = "Sample Label";
            labelControl.PicturePosition = ControlPicturePositionType.LeftTop;

            // Läs in en bild för Picture-egenskapen
            string imagePath = "sample.jpg"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                labelControl.Picture = File.ReadAllBytes(imagePath);
                Console.WriteLine("Picture set successfully");
            }
            else
            {
                Console.WriteLine("Image file not found, using null picture");
                labelControl.Picture = null;
            }

            // Spara arbetsboken
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


