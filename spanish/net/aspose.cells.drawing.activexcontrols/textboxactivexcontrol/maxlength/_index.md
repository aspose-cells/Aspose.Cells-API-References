---
title: "TextBoxActiveXControl.MaxLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece el número máximo de caracteres"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

Obtiene y establece el número máximo de caracteres

```csharp
public int MaxLength { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox y obtener su propiedad ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad MaxLength
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


