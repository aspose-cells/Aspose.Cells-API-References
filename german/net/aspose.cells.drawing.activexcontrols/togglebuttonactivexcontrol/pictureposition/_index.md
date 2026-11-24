---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl Eigenschaft. Ruft den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Liest und setzt den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Beispiele

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

            // Füge ein ToggleButton ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Setze die PicturePosition‑Eigenschaft
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Setze weitere Eigenschaften, um die Funktionalität zu demonstrieren
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


