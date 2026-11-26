---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButtonActiveXControl. Obtiene y establece la posición de la leyenda relativa al control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Obtiene y establece la posición del Caption relativo al control.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una nueva colección de formas y agregar control ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Establecer la propiedad Alignment
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Guarda el libro de trabajo
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


