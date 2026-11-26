---
title: "RadioButton.IsChecked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButton. Indica si el radiobutton está marcado o no"
type: docs
url: /es/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Indica si el botón de opción está marcado o no.

```csharp
public bool IsChecked { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un radio button a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Establecer el texto del radio button
            radioButton.Text = "Option 1";
            
            // Inicialmente sin marcar
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Marcar el radio button
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Guarda el libro de trabajo
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Ver también

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


