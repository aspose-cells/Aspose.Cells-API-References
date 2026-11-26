---
title: "ActiveXControl.IsTransparent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Indica si el control es transparente"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Indica si el control es transparente.

```csharp
public bool IsTransparent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para alojar el control ActiveX con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Establecer propiedades del control
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Verificar y mostrar la propiedad IsTransparent
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Cambiar la transparencia y verificar nuevamente
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


