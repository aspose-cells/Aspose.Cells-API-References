---
title: "CommandButtonActiveXControl.Caption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommandButtonActiveXControl-egenskap. Hämtar och anger den beskrivande texten som visas på en kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/
---
## CommandButtonActiveXControl.Caption property

Hämtar och anger den beskrivande texten som visas på en kontroll.

```csharp
public string Caption { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl commandButton = (Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl)shape.ActiveXControl;

            // Demonstrera användning av Caption‑egenskapen
            commandButton.Caption = "Click Me";
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);

            workbook.Save("CommandButtonCaptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


