---
title: "LabelActiveXControl.BorderStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LabelActiveXControl-Eigenschaft. Liest und schreibt den Typ des vom Steuerelement verwendeten Rahmens"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderstyle/
---
## LabelActiveXControl.BorderStyle property

Liest und schreibt den Typ des vom Steuerelement verwendeten Rahmens.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Border Style Demo";
            label.BorderStyle = ControlBorderType.Single;
            label.BorderOleColor = 0xFF0000; // Red border

            Console.WriteLine("Label Border Style: " + label.BorderStyle);
            Console.WriteLine("Label Border Color: " + label.BorderOleColor);

            workbook.Save("LabelBorderStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlBorderType](../../controlbordertype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


