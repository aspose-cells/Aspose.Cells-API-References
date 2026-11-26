---
title: "Clase CustomGeometry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.CustomGeometry. Representa una forma geométrica personalizada"
type: docs
url: /es/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Representa una forma geométrica personalizada.

```csharp
public class CustomGeometry : Geometry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Obtiene información de la colección de rutas cuando la forma es un autoshape NotPrimitive |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Obtiene una colección de valores de ajuste de forma (heredado de [`Geometry`](../geometry/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un autoshape NotPrimitive con los parámetros correctos
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Obtener la instancia de CustomGeometry de la forma
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Crear una nueva ruta en la colección de rutas de la geometría
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Agregar segmentos de ruta usando llamadas directas a métodos
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Guarda el libro de trabajo
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


