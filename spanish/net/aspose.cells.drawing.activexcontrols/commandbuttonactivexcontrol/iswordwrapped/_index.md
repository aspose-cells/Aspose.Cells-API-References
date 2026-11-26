---
title: "CommandButtonActiveXControl.IsWordWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Indica si el contenido del control se ajusta automáticamente al final de una línea"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/
---
## CommandButtonActiveXControl.IsWordWrapped property

Indica si el contenido del control se ajusta automáticamente al final de una línea.

```csharp
public bool IsWordWrapped { get; set; }
```

### Ejemplos

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

### Ver también

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


