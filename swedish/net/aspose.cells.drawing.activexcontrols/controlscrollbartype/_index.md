---
title: "Enum ControlScrollBarType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType enum. Representerar typen av rullningslist"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Representerar typen av rullningslist.

```csharp
public enum ControlScrollBarType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Visar inga rullningslister. |
| Horizontal | `1` | Visar en horisontell rullningslist. |
| BarsVertical | `2` | Visar en vertikal rullningslist. |
| BarsBoth | `3` | Visar både en horisontell och en vertikal rullningslist. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX‑kontroll i kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Ange ScrollBars-egenskapen för att visa både horisontella och vertikala rullningslister
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Spara arbetsboken
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


