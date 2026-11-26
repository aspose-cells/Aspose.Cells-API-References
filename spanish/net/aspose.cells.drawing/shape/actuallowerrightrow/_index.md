---
title: "Shape.ActualLowerRightRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtenga la fila inferior real"
type: docs
url: /es/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Obtener la fila inferior real.

```csharp
public int ActualLowerRightRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma de muestra (rectángulo)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Obtenga la fila inferior derecha real de la forma
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Mostrar el resultado
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


