---
title: "ActiveXControlBase.MousePointer"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger typen av ikon som visas som muspekare för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Hämtar och anger typen av ikon som visas som muspekare för kontrollen.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Exempel

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

### Se även

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


