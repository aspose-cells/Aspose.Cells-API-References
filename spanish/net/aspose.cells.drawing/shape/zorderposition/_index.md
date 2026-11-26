---
title: "Shape.ZOrderPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Devuelve la posición de una forma en el z‑order"
type: docs
url: /es/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Devuelve la posición de una forma en el orden Z.

```csharp
public int ZOrderPosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar tres formas para demostrar ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // Establecer posiciones ZOrder
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // Cambiar ZOrder de shape3 para llevarla al frente
            shape3.ZOrderPosition = 0;

            // Guarda el libro de trabajo
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


