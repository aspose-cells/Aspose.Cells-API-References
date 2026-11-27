---
title: "CommandButtonActiveXControl.TakeFocusOnClick"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommandButtonActiveXControl egenskap. Anger om kontrollen tar fokus när den klickas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/
---
## CommandButtonActiveXControl.TakeFocusOnClick property

Anger om kontrollen får fokus när den klickas.

```csharp
public bool TakeFocusOnClick { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyTakeFocusOnClickDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Click Me";
            commandButton.TakeFocusOnClick = true;
            
            workbook.Save("CommandButtonActiveXControlTakeFocusOnClickDemo.xlsx");
        }
    }
}
```

### Se även

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


