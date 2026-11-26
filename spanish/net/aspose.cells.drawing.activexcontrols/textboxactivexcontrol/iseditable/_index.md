---
title: "TextBoxActiveXControl.IsEditable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el usuario puede escribir en el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/
---
## TextBoxActiveXControl.IsEditable property

Indica si el usuario puede escribir en el control.

```csharp
public bool IsEditable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demuestra la propiedad IsEditable
            Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
            
            // Alterna la propiedad IsEditable
            textBox.IsEditable = !textBox.IsEditable;
            Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);

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


