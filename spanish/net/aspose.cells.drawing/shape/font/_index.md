---
title: "Shape.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la fuente de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Representa la fuente de la forma.

```csharp
public Font Font { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Acceder y modificar las propiedades de fuente de la forma
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


