---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Indica si se rota el texto con la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Indica si se rota el texto con la forma.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto con los parámetros correctos
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Acceder a las propiedades de alineación de texto
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Establecer la propiedad RotateTextWithShape
            textAlignment.RotateTextWithShape = true;

            // Rota la forma para demostrar el efecto
            shape.RotationAngle = 45;

            // Guarda el libro de trabajo
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


