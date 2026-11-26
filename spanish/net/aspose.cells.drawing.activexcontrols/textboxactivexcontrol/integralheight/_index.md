---
title: "TextBoxActiveXControl.IntegralHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el control mostrará solo líneas completas de texto sin mostrar líneas parciales"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/
---
## TextBoxActiveXControl.IntegralHeight property

Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales.

```csharp
public bool IntegralHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control ActiveX TextBox y obtén su propiedad ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demuestra la propiedad IntegralHeight
            Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
            
            // Establece IntegralHeight a true si está en false
            if (!textBox.IntegralHeight)
            {
                textBox.IntegralHeight = true;
                Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


