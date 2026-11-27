---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar och anger om SpinButton eller ScrollBar är orienterad vertikalt eller horisontellt"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

Hämtar och anger om SpinButton eller ScrollBar är orienterad vertikalt eller horisontellt.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Exempel

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

            // Lägg till en SpinButton ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Kontrollera och ändra orientering
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Spara arbetsboken
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


