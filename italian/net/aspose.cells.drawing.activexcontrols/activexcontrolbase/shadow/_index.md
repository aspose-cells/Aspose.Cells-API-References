---
title: "ActiveXControlBase.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ActiveXControlBase proprietà. Indica se mostrare un'ombra"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/
---
## ActiveXControlBase.Shadow property

Indica se mostrare un'ombra.

```csharp
public virtual bool Shadow { get; set; }
```

### Esempi

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

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


