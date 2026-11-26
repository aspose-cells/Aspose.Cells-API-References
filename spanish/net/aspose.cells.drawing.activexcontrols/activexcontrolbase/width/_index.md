---
title: "ActiveXControlBase.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece el ancho del control en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/width/
---
## ActiveXControlBase.Width property

Obtiene y establece el ancho del control en unidades de puntos.

```csharp
public virtual double Width { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;

            // Demostrar el uso de la propiedad Width
            Console.WriteLine("Original width: " + control.Width);
            control.Width = 150;
            Console.WriteLine("Modified width: " + control.Width);

            workbook.Save("ActiveXControlWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


