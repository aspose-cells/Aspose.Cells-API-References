---
title: "Shape.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el tipo de forma automática"
type: docs
url: /es/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Obtiene el tipo de forma automática.

```csharp
public AutoShapeType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Obtener y mostrar el tipo de forma
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // No se puede cambiar el tipo de forma ya que la propiedad Type es de solo lectura
            // En su lugar, crea una nueva forma con un tipo diferente
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### Ver también

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


