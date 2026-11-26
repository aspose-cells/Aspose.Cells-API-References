---
title: "CustomGeometry.Paths"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomGeometry. Obtiene información de la colección de rutas cuando la forma es un autoshape NotPrimitive"
type: docs
url: /es/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Obtiene información de la colección de rutas cuando la forma es un autoshape NotPrimitive

```csharp
public ShapePathCollection Paths { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma personalizada con geometría no primitiva (parámetros fijos)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Acceder a la geometría personalizada mediante conversión explícita
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Obtener colección de rutas
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Crear una nueva ruta de forma usando comandos de dibujo
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // No se necesita Add explícito ya que la ruta se creó en la colección
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Guardar para demostrar cambios persistentes
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


