---
title: "RadioButtonActiveXControl.IsWordWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButtonActiveXControl. Indica si el contenido del control se ajusta automáticamente al final de una línea"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/iswordwrapped/
---
## RadioButtonActiveXControl.IsWordWrapped property

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
    public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX RadioButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton = 
                (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad IsWordWrapped
            Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = true;
            Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = false;
            Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);

            // Guarda el libro de trabajo
            workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


