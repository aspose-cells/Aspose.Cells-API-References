---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpinButtonActiveXControl-Eigenschaft. Gibt an und legt fest, ob der SpinButton oder die ScrollBar vertikal oder horizontal ausgerichtet ist"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

Liest und setzt, ob der SpinButton oder ScrollBar vertikal oder horizontal ausgerichtet ist.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyOrientationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein SpinButton‑ActiveX‑Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Überprüfen und ändern Sie die Ausrichtung
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


