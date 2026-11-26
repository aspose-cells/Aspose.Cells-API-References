---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece el tipo de borde utilizado por el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

Obtiene y establece el tipo de borde utilizado por el control.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Establece la propiedad BorderStyle
            textBox.BorderStyle = ControlBorderType.Single;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


