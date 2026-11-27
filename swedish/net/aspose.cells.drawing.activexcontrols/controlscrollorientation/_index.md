---
title: "Enum ControlScrollOrientation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation enum. Representerar typ av rullningsorientering"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Representerar typ av rullningsorientering

```csharp
public enum ControlScrollOrientation
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Auto | `3` | Kontrollen renderas horisontellt när kontrollens bredd är större än dess höjd. Kontrollen renderas vertikalt annars. |
| Vertical | `0` | Kontrollen renderas vertikalt. |
| Horizontal | `1` | Kontrollen renderas horisontellt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ScrollBarActiveXControl till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Demonstrera hur man ställer in orienteringen med hjälp av ControlScrollOrientation enum
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Spara arbetsboken
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


