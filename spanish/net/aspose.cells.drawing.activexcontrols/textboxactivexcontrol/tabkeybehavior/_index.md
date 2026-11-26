---
title: "TextBoxActiveXControl.TabKeyBehavior"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si se permiten caracteres de tabulación en el texto del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/
---
## TextBoxActiveXControl.TabKeyBehavior property

Indica si se permiten caracteres de tabulación en el texto del control.

```csharp
public bool TabKeyBehavior { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox y obtener su propiedad ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad TabKeyBehavior
            Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
            
            // Habilitar TabKeyBehavior
            if (!textBoxControl.TabKeyBehavior)
            {
                textBoxControl.TabKeyBehavior = true;
                Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


