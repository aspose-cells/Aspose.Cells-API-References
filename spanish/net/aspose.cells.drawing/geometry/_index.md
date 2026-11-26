---
title: "Clase Geometry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Geometry. Representa una forma geométrica"
type: docs
url: /es/net/aspose.cells.drawing/geometry/
---
## Geometry class

Representa una forma geométrica.

```csharp
public abstract class Geometry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Obtiene una colección de valores de ajuste de forma |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Acceder a la geometría de la forma
            Geometry geometry = rectangle.Geometry;

            // Agregar guías de ajuste de forma directamente a la colección
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Guardar el libro de trabajo modificado
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


