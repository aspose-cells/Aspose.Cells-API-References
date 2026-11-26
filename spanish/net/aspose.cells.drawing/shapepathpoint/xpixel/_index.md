---
title: "ShapePathPoint.XPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPoint. Cuando el objeto es una coordenada de posición, obtener o establecer la coordenada x en píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles.

```csharp
public int XPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Agregar puntos con coordenadas
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Acceder al primer punto y demostrar la propiedad XPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Mostrar el valor de XPixel (operación de lectura)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Establecer un nuevo valor para XPixel (ya que es de lectura/escritura)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Crear una ruta de forma y agregar los puntos
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Agregar el segundo punto
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

                // Agrega una forma libre a la hoja de cálculo
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Guarda el libro de trabajo
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


