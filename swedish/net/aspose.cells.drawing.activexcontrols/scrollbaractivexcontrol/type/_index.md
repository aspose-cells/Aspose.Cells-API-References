---
title: "ScrollBarActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBarActiveXControl-egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ScrollBar ActiveX-kontroll med korrekta parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Kontrollera kontrollens typ med Type-egenskapen
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Ange ScrollBar-specifika egenskaper
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Spara arbetsboken
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


