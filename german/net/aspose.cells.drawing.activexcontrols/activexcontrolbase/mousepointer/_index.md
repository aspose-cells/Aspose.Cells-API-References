---
title: "ActiveXControlBase.MousePointer"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt den Typ des Icons, das als Mauszeiger für das Steuerelement angezeigt wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Ruft den Typ des als Mauszeiger für das Steuerelement angezeigten Symbols ab und legt ihn fest.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyMousePointerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 50);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "Click Me";
            button.MousePointer = ControlMousePointerType.Help;
            button.MouseIcon = new byte[] { }; // Empty byte array for custom icon (when MousePointer is Custom)
            
            workbook.Save("ActiveXControlMousePointerDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


