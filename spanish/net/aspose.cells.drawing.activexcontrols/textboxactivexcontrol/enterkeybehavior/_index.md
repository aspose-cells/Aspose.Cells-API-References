---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Especifica el comportamiento de la tecla ENTER. True indica que al presionar ENTER se creará una nueva línea. False indica que al presionar ENTER se moverá el foco al siguiente objeto en el orden de tabulación"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

Especifica el comportamiento de la tecla ENTER. True especifica que al presionar ENTER se creará una nueva línea. False especifica que al presionar ENTER se moverá el foco al siguiente objeto en el orden de tabulación.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterKeyBehaviorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad EnterKeyBehavior
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // Alternar el EnterKeyBehavior
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

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


