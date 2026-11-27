---
title: "ToggleButtonActiveXControl.Picture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Hämtar och anger bildens data"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Hämtar och anger bildens data.

```csharp
public byte[] Picture { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX‑kontroll och hämta dess ActiveXControl‑egenskap
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Ange bild för växlingsknappen
            byte[] data = File.ReadAllBytes("image.png");
            toggleButton.Picture = data;

            // Spara arbetsboken
            workbook.Save("ToggleButtonWithPicture.xlsx");
        }
    }
}
```

### Se även

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


