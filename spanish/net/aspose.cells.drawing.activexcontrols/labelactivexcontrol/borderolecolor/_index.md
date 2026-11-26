---
title: "LabelActiveXControl.BorderOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece el color ole del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public int BorderOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX Label
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl = 
                (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            // Establecer propiedades
            labelControl.Caption = "Sample Label";
            labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
            labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Guarda el libro de trabajo
            workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");

            // Mostrar el color del borde
            Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
        }
    }
}
```

### Ver también

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


