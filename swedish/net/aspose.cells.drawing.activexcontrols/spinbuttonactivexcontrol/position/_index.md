---
title: "SpinButtonActiveXControl.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar och anger värdet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Hämtar och anger värdet.

```csharp
public int Position { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en SpinButton ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // Hämta ActiveX-kontrollen och ange Position-egenskapen
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Spara arbetsboken
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### Se även

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


