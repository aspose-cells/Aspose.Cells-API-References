---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBarActiveXControl-Eigenschaft. Ruft die Menge ab, um die sich die Position-Eigenschaft ändert, und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Liest und setzt den Betrag, um den sich die Position‑Eigenschaft ändert

```csharp
public int LargeChange { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ScrollBar ActiveX-Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Setzen Sie die LargeChange-Eigenschaft
            scrollBar.LargeChange = 5;

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


