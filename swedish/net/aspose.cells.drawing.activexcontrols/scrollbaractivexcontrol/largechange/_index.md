---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBarActiveXControl-egenskap. Hämtar och anger mängden som Position-egenskapen förändras med"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Hämtar och anger mängden som Position-egenskapen ändras med

```csharp
public int LargeChange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ScrollBar ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Ange LargeChange-egenskapen
            scrollBar.LargeChange = 5;

            // Spara arbetsboken
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


