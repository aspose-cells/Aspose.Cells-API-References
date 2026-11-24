---
title: "Shape.ActiveXControl"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt das ActiveX-Steuerelement zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/activexcontrol/
---
## Shape.ActiveXControl property

Ruft das ActiveX-Steuerelement ab.

```csharp
public ActiveXControl ActiveXControl { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ShapePropertyActiveXControlDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 0, 0, 0, 100, 30);

            if (shape.ActiveXControl != null)
            {
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                string fontName = checkBox.Font.Name;
                Console.WriteLine($"CheckBox Font: {fontName}");
            }
        }
    }
}
```

### Siehe auch

* class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


