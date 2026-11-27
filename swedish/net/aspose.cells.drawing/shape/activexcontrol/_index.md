---
title: "Shape.ActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar ActiveX‑kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/activexcontrol/
---
## Shape.ActiveXControl property

Hämtar ActiveX-kontrollen.

```csharp
public ActiveXControl ActiveXControl { get; }
```

### Exempel

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

### Se även

* class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


