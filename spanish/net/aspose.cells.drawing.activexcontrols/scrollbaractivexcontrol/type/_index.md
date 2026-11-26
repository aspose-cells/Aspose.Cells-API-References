---
title: "ScrollBarActiveXControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBarActiveXControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ScrollBar con los parámetros correctos
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Verifique el tipo de control usando la propiedad Type
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Establecer propiedades específicas del ScrollBar
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


