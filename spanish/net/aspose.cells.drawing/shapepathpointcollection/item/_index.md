---
title: "ShapePathPointCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPointCollection. Obtiene el punto de ruta de la forma por índice"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpointcollection/item/
---
## ShapePathPointCollection indexer

Obtiene el punto de la ruta de la forma por índice.

```csharp
public ShapePathPoint this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice |

### Valor de retorno

Devuelve el objeto [`ShapePathPoint`](../../shapepathpoint/)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una colección de puntos de ruta de forma y agregue puntos
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Acceda a los puntos usando la propiedad Item
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Cree una ruta de forma usando los puntos
            ShapePath path = new ShapePath();

            // Mover al punto de inicio
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Agregue una forma libre con la ruta configurada
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Guardar el resultado
            workbook.Save("ShapePathPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePathPoint](../../shapepathpoint/)
* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


