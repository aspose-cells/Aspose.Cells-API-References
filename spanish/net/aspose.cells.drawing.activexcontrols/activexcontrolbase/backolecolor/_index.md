---
title: "ActiveXControlBase.BackOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece el color ole del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/
---
## ActiveXControlBase.BackOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public virtual int BackOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyBackOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "BackOleColor Demo";
            label.BackOleColor = 0xFFFF00; // Yellow background
            label.ForeOleColor = 0x0000FF; // Blue text
            label.IsAutoSize = true;

            Console.WriteLine("Label Back Color: " + label.BackOleColor.ToString("X6"));
            
            workbook.Save("BackOleColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


