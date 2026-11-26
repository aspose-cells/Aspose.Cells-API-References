---
title: "TextBoxActiveXControl.IsMultiLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el control puede mostrar más de una línea de texto"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/
---
## TextBoxActiveXControl.IsMultiLine property

Indica si el control puede mostrar más de una línea de texto.

```csharp
public bool IsMultiLine { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsMultiLineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad IsMultiLine
            if (!textBox.IsMultiLine)
            {
                textBox.IsMultiLine = true;
                textBox.Text = "This is a multi-line text box.\nSecond line of text.";
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


