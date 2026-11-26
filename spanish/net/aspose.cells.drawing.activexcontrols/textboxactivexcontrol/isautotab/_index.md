---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres.

```csharp
public bool IsAutoTab { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox y obtener su control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad IsAutoTab
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // Establecer IsAutoTab a verdadero si está en falso
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


