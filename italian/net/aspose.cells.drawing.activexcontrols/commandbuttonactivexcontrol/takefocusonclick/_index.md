---
title: "CommandButtonActiveXControl.TakeFocusOnClick"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CommandButtonActiveXControl proprietà. Indica se il controllo prende il focus quando viene cliccato"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/
---
## CommandButtonActiveXControl.TakeFocusOnClick property

Indica se il controllo prende il focus quando viene cliccato.

```csharp
public bool TakeFocusOnClick { get; set; }
```

### Esempi

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

### Vedi anche

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


