---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpinButtonActiveXControl. Obtiene y establece si el SpinButton o ScrollBar está orientado vertical u horizontalmente"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

Obtiene y establece si el SpinButton o ScrollBar está orientado vertical u horizontalmente.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyOrientationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX SpinButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Verifica y modifica la orientación
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Guarda el libro de trabajo
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


