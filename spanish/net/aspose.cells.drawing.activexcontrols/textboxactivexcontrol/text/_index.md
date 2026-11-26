---
title: "TextBoxActiveXControl.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece el texto del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/
---
## TextBoxActiveXControl.Text property

Obtiene y establece el texto del control.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un control ActiveX TextBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            
            // Obtén el control ActiveX y establece su texto
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
            textBox.Text = "This is a test.";
            
            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


