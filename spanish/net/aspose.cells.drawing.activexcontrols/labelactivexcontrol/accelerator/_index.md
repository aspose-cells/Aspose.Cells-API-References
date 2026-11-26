---
title: "LabelActiveXControl.Accelerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece la tecla aceleradora del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/accelerator/
---
## LabelActiveXControl.Accelerator property

Obtiene y establece la tecla de acceso rápido para el control.

```csharp
public char Accelerator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Press Alt+H";
            label.Accelerator = 'H';
            label.IsVisible = true;

            Console.WriteLine("Label Caption: " + label.Caption);
            Console.WriteLine("Label Accelerator: " + label.Accelerator);

            workbook.Save("LabelActiveXControlAcceleratorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


