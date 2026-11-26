---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScrollBarActiveXControl. Obtiene y establece la cantidad en que cambia la propiedad Position"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Obtiene y establece la cantidad en que cambia la propiedad Position

```csharp
public int LargeChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ScrollBar
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad LargeChange
            scrollBar.LargeChange = 5;

            // Guarda el libro de trabajo
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


