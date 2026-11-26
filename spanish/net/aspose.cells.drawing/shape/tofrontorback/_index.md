---
title: "Shape.ToFrontOrBack"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Lleva la forma al frente o la envía al fondo"
type: docs
url: /es/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Trae la forma al frente o envía la forma al fondo.

```csharp
public void ToFrontOrBack(int orders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| órdenes | Int32 | Si es menor que cero, coloca la forma al fondo. Si es mayor que cero, lleva la forma al frente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue dos formas para demostrar el orden Z
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Mueva shape2 2 posiciones hacia adelante en el orden Z
            shape2.ToFrontOrBack(2);

            // Mueva shape1 1 posición hacia atrás en el orden Z
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


