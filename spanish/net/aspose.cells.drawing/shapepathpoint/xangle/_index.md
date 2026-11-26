---
title: "ShapePathPoint.XAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePathPoint. Cuando el objeto es un marcador de ángulo, obtener o establecer el primer ángulo en grados"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados.

```csharp
public int XAngle { get; set; }
```

### Observaciones

Si este ángulo es el ángulo inicial de un arco. Este ángulo especificará qué ángulo a lo largo de la supuesta ruta circular se usará como posición inicial para dibujar el arco. Este ángulo inicial se bloqueará a la última posición conocida del lápiz en la ruta de forma. Así se garantiza una ruta de forma continua.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una colección de puntos de ruta de forma
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Recuperar el primer punto y mostrar sus coordenadas X e Y
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // NOTA: La clase ShapePathPoint (según la reflexión actual de la API) no expone una propiedad XAngle.
            // Por lo tanto, esta demostración se centra en las propiedades X e Y disponibles.

            // Construir una forma libre simple usando los puntos definidos
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Agregar la forma libre a la hoja de cálculo
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Guarda el libro de trabajo
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


