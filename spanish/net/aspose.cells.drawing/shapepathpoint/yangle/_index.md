---
title: "ShapePathPoint.YAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPoint. Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados.

```csharp
public int YAngle { get; set; }
```

### Observaciones

Si este ángulo es el ángulo de oscilación de un arco. Este ángulo especificará cuán lejos, en términos angulares, a lo largo de la supuesta trayectoria circular se extenderá el arco. La extensión desde el ángulo inicial siempre será en dirección horaria alrededor del supuesto círculo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // Agregue puntos con marcadores de ángulo (usando XAngle y YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Muestre el valor de YAngle
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Crear otro punto con diferentes ángulos
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Muestre el valor de YAngle
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Crear una ruta de forma y agregar arco usando marcadores de ángulo
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

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
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


