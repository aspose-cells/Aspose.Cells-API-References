---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Hämtar och anger platsen för kontrollens bild relativt dess rubrik"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Hämtar och anger placeringen av kontrollens bild i förhållande till dess rubrik.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX‑kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Ange PicturePosition‑egenskap
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Ange andra egenskaper för att demonstrera funktionaliteten
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Spara arbetsboken
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


