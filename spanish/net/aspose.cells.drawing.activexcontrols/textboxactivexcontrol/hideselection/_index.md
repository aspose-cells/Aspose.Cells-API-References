---
title: "TextBoxActiveXControl.HideSelection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/
---
## TextBoxActiveXControl.HideSelection property

Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco.

```csharp
public bool HideSelection { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad HideSelection
            Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
            
            // Establecer HideSelection a true si está en false
            if (!textBox.HideSelection)
            {
                textBox.HideSelection = true;
                Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


