---
title: "Clase ShapeSegmentPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ShapeSegmentPath. Representa una ruta de segmento en una ruta del trazado libre"
type: docs
url: /es/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Representa una ruta de segmento en una ruta del trazado libre.

```csharp
public class ShapeSegmentPath
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Obtiene los puntos en el segmento de ruta |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Obtiene el tipo de segmento de ruta |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma libre a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Obtén la ruta geométrica de la forma
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Accede a la primera ruta de segmento (si existe)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Demuestra las propiedades de ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Itera a través de los puntos en la ruta de segmento
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


