---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Especifica el comportamiento de selección al entrar al control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar al control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Especifica el comportamiento de selección al entrar al control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar al control.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control TextBox ActiveX con los parámetros correctos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demuestra la propiedad EnterFieldBehavior
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Alterna la propiedad EnterFieldBehavior
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Establece EnterFieldBehavior a true explícitamente
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


