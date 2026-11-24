---
title: "ScrollBarActiveXControl.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBarActiveXControl-Eigenschaft. Ruft den Typ des ActiveX-Steuerelements ab"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

Liest den Typ des ActiveX-Steuerelements.

```csharp
public override ControlType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ScrollBar ActiveX-Steuerelement mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Überprüfen Sie den Steuertyp mithilfe der Type-Eigenschaft
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Setzen Sie spezifische ScrollBar-Eigenschaften
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


