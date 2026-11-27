---
title: "ToggleButtonActiveXControl.Caption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Hämtar och anger den beskrivande texten som visas på en kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption/
---
## ToggleButtonActiveXControl.Caption property

Hämtar och anger den beskrivande texten som visas på en kontroll.

```csharp
public string Caption { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 2, 0, 2, 0, 100, 30);
            ToggleButtonActiveXControl toggleButtonControl = (ToggleButtonActiveXControl)shape.ActiveXControl;
            toggleButtonControl.Caption = "ExampleButton";

            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


