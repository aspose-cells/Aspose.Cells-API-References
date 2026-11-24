---
title: "CommandButtonActiveXControl.TakeFocusOnClick"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommandButtonActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement beim Klicken den Fokus erhält"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/
---
## CommandButtonActiveXControl.TakeFocusOnClick property

Gibt an, ob das Steuerelement beim Klicken den Fokus erhält.

```csharp
public bool TakeFocusOnClick { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


