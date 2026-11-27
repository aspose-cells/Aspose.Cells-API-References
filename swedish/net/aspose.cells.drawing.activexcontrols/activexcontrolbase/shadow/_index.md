---
title: "ActiveXControlBase.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Anger om en skugga ska visas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/
---
## ActiveXControlBase.Shadow property

Anger om en skugga ska visas.

```csharp
public virtual bool Shadow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Shadow Button";
            commandButton.Shadow = true;

            workbook.Save("ActiveXControlShadowDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


