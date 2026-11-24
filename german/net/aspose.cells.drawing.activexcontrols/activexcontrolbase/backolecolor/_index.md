---
title: "ActiveXControlBase.BackOleColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt die Ole-Farbe des Hintergrunds"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/
---
## ActiveXControlBase.BackOleColor property

Liest und schreibt die OLE-Farbe des Hintergrunds.

```csharp
public virtual int BackOleColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyBackOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "BackOleColor Demo";
            label.BackOleColor = 0xFFFF00; // Yellow background
            label.ForeOleColor = 0x0000FF; // Blue text
            label.IsAutoSize = true;

            Console.WriteLine("Label Back Color: " + label.BackOleColor.ToString("X6"));
            
            workbook.Save("BackOleColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


