---
title: "ToggleButtonActiveXControl.Picture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl Eigenschaft. Ruft die Daten des Bildes ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Liest und setzt die Bilddaten.

```csharp
public byte[] Picture { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ToggleButton ActiveX-Steuerelement hinzu und rufe dessen ActiveXControl‑Eigenschaft ab
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Setze das Bild für die Umschalt-Schaltfläche
            byte[] data = File.ReadAllBytes("image.png");
            toggleButton.Picture = data;

            // Speichere die Arbeitsmappe
            workbook.Save("ToggleButtonWithPicture.xlsx");
        }
    }
}
```

### Siehe auch

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


