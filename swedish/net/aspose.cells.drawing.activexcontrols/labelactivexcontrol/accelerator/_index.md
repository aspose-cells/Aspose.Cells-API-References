---
title: "LabelActiveXControl.Accelerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl egenskap. Hämtar och anger acceleratortangenten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/accelerator/
---
## LabelActiveXControl.Accelerator property

Hämtar och anger acceleratortangenten för kontrollen.

```csharp
public char Accelerator { get; set; }
```

### Exempel

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

### Se även

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


