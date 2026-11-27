---
title: "CommandButtonActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommandButtonActiveXControl egenskap. Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/
---
## CommandButtonActiveXControl.IsWordWrapped property

Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 2, 2, 150, 30);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "Click to demonstrate word wrapping in caption";
            button.IsWordWrapped = true;

            workbook.Save("CommandButtonIsWordWrappedDemo.xlsm");
        }
    }
}
```

### Se även

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


