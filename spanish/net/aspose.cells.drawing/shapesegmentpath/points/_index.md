---
title: "ShapeSegmentPath.Points"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeSegmentPath. Obtiene los puntos en el segmento de ruta"
type: docs
url: /es/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Obtiene los puntos en el segmento de ruta

```csharp
public ShapePathPointCollection Points { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Inicia una nueva ruta
            path.MoveTo(10, 10);

            // Dibuja un segmento de línea
            path.LineTo(100, 100);

            // Acceder a la propiedad PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Acceder a la primera ruta del segmento
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Mostrar información de los puntos
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //agregar forma libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Guarda el libro de trabajo
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


