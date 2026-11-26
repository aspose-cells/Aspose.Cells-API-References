---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una nueva colección de formas y agregar control ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Establecer la propiedad ScrollBars a vertical
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Guarda el libro de trabajo
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


