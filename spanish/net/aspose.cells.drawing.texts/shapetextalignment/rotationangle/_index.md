---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece la rotación de la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Obtiene y establece la rotación de la forma.

```csharp
public double RotationAngle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Establecer texto de la forma
            shape.Text = "Rotated Text";
            
            // Acceder a la alineación de texto y establecer el ángulo de rotación
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


