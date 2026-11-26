---
title: "ShapePathPoint.YPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPoint. Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles.

```csharp
public int YPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
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

                // Agregue un punto con coordenadas
                pathPoints.Add(100, 50);

                // Acceda al primer punto y demuestre la propiedad YPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Muestre el valor inicial de YPixel (operación de lectura)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Establezca un nuevo valor para YPixel (ya que es de lectura/escritura)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Cree una ruta de forma y use el punto
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

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
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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


