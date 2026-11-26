---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Obtiene o establece la dirección de visualización del texto dentro de un cuerpo de texto dado. Corresponde a Format Shape  Text Options  Text Box  Text direction en Excel"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Obtiene o establece la dirección de visualización del texto dentro de un cuerpo de texto dado. Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Dirección del texto" en Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Establecer la dirección del texto a vertical
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Establecer algún texto para demostrar la dirección
            shape.Text = "Vertical Text Example";

            // Guarda el libro de trabajo
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


