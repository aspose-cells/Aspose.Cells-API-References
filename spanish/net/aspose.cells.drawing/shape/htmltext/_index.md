---
title: "Shape.HtmlText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece la cadena HTML que contiene datos y algunos formatos en este cuadro de texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Obtiene y establece la cadena html que contiene datos y algunos formatos en este cuadro de texto.

```csharp
public string HtmlText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Verifique si HtmlText está vacío y establézcalo si es necesario
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


