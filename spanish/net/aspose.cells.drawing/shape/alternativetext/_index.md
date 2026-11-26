---
title: "Shape.AlternativeText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Devuelve o establece la cadena de texto alternativa descriptiva del objeto Shape"
type: docs
url: /es/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Devuelve o establece la cadena de texto descriptiva (alternativa) del objeto [`Shape`](../).

```csharp
public string AlternativeText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Establecer texto alternativo para la forma
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Guarda el libro de trabajo
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


