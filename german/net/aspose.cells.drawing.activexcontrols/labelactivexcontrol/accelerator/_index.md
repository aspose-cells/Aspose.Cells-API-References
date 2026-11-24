---
title: "LabelActiveXControl.Accelerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LabelActiveXControl-Eigenschaft. Liest und schreibt die Beschleunigungstaste für das Steuerelement"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/accelerator/
---
## LabelActiveXControl.Accelerator property

Liest und setzt die Beschleunigungstaste für das Steuerelement.

```csharp
public char Accelerator { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Press Alt+H";
            label.Accelerator = 'H';
            label.IsVisible = true;

            Console.WriteLine("Label Caption: " + label.Caption);
            Console.WriteLine("Label Accelerator: " + label.Accelerator);

            workbook.Save("LabelActiveXControlAcceleratorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


