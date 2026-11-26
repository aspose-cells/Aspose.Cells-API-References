---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Especifica el símbolo que se muestra en el botón desplegable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Especifica el símbolo mostrado en el botón desplegable

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyDropButtonStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega un control TextBox ActiveX
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Convierte a TextBoxActiveXControl para acceder a las propiedades específicas de TextBox
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Establece la propiedad DropButtonStyle
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


