---
title: "TextBoxActiveXControl.IsWordWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el contenido del control se ajusta automáticamente al final de una línea"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/
---
## TextBoxActiveXControl.IsWordWrapped property

Indica si el contenido del control se ajusta automáticamente al final de una línea.

```csharp
public bool IsWordWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer un texto que se beneficiaría del ajuste de línea
            textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";

            // Verificar y establecer la propiedad IsWordWrapped
            if (!textBox.IsWordWrapped)
            {
                textBox.IsWordWrapped = true;
                Console.WriteLine("Word wrapping has been enabled for the TextBox.");
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


