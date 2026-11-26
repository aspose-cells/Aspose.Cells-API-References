---
title: "ShapeTextAlignment.TextVerticalType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece la dirección del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/textverticaltype/
---
## ShapeTextAlignment.TextVerticalType property

Obtiene y establece la dirección del texto.

```csharp
public TextVerticalType TextVerticalType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto con los parámetros correctos
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Obtener la alineación de texto y establecer el tipo de texto vertical
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Guarda el libro de trabajo
            workbook.Save("TextVerticalTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


