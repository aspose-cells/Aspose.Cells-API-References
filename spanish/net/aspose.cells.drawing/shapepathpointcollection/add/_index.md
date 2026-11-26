---
title: "ShapePathPointCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePathPointCollection. Añade un punto de ruta en unidades EMU"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Añade un punto de ruta en unidades EMU.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| x | Int32 | La coordenada x. |
| y | Int32 | La coordenada y. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice los métodos MoveTo,LineTo,CubicBezierTo y ArcTo en ShapePath. Este método será eliminado 12 meses después, a partir de agosto de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una colección de puntos de ruta de forma
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Llame al método Add con parámetros (Int32, Int32)
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Crear una ruta de forma y agregar los puntos
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
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


