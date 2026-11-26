---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece un carácter que se mostrará en lugar de los caracteres ingresados"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

Obtiene y establece un carácter que se mostrará en lugar de los caracteres ingresados.

```csharp
public char PasswordChar { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox y obtener su forma
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // Obtener el TextBoxActiveXControl de la forma
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad PasswordChar
            textBoxControl.PasswordChar = '*';

            // Establecer algún texto para demostrar el enmascaramiento de contraseña
            textBoxControl.Text = "password123";

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


