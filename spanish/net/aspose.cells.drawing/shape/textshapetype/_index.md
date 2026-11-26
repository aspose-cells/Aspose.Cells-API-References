---
title: "Shape.TextShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el tipo de shape de texto predefinido"
type: docs
url: /es/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Obtiene y establece el tipo de forma de texto predefinido.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Verificar y establecer TextShapeType si es desconocido
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Mostrar el TextShapeType de la forma
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### Ver también

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


