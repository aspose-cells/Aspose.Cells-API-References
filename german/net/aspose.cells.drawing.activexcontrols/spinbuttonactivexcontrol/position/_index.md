---
title: "SpinButtonActiveXControl.Position"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpinButtonActiveXControl-Eigenschaft. Liest und schreibt den Wert"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Liest und setzt den Wert.

```csharp
public int Position { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein SpinButton‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // Hole das ActiveX-Steuerelement und setze die Position-Eigenschaft
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Speichere die Arbeitsmappe
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


