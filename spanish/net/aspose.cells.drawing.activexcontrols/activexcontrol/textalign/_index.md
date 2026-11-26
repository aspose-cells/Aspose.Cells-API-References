---
title: "ActiveXControl.TextAlign"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Representa cómo alinear el texto usado por el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

Representa cómo alinear el texto usado por el control.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyTextAlignDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar dos controles ActiveX de casilla de verificación
            Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
            Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);

            // Obtener los controles ActiveX
            CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
            CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;

            // Establecer diferentes alineaciones de texto
            checkbox1.TextAlign = TextAlignmentType.Center;
            checkbox2.TextAlign = TextAlignmentType.Right;

            // Mostrar los valores de alineación de texto
            Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
            Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


