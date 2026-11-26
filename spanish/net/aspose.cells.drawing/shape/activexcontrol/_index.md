---
title: "Shape.ActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing/shape/activexcontrol/
---
## Shape.ActiveXControl property

Obtiene el control ActiveX.

```csharp
public ActiveXControl ActiveXControl { get; }
```

### Ejemplos

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

### Ver también

* class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


