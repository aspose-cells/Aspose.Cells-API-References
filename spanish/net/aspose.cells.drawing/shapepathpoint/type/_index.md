---
title: "ShapePathPoint.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPoint. Especifica el tipo de valor del objeto actual"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/type/
---
## ShapePathPoint.Type property

Especifica el tipo de valor del objeto actual.

```csharp
public ShapePathPointValueType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Cree una colección de puntos de ruta de forma
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Agregar un punto de coordenada de posición
                int positionPointIndex = pathPoints.Add(100, 50);
                ShapePathPoint positionPoint = pathPoints[positionPointIndex];

                // Mostrar el valor de la propiedad Type para la coordenada de posición
                Console.WriteLine($"Position Point Type: {positionPoint.Type}");
                Console.WriteLine($"Position Point Type is Position: {positionPoint.Type == ShapePathPointValueType.Position}");

                // Agregar un punto marcador de ángulo
                int anglePointIndex = pathPoints.Add(0, 0);
                ShapePathPoint anglePoint = pathPoints[anglePointIndex];
                anglePoint.XAngle = 45;
                anglePoint.YAngle = 90;

                // Mostrar el valor de la propiedad Type para el marcador de ángulo
                Console.WriteLine($"Angle Point Type: {anglePoint.Type}");
                Console.WriteLine($"Angle Point Type is Angle: {anglePoint.Type == ShapePathPointValueType.Angle}");

                // Crear una ruta de forma y agregar puntos
                ShapePath path = new ShapePath();
                path.MoveTo(positionPoint.XPixel, positionPoint.YPixel);
                path.ArcTo(anglePoint.XAngle, anglePoint.YAngle, 100, 100);
                path.Close();

                // Añadir forma libre a la hoja de cálculo
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Guarda el libro de trabajo
                workbook.Save("ShapePathPointTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [ShapePathPointValueType](../../shapepathpointvaluetype/)
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


