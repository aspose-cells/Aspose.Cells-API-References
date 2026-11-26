---
title: "Enum ShapePathType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ShapePathType enum. Representa el tipo de segmento de ruta"
type: docs
url: /es/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Representa el tipo de segmento de ruta.

```csharp
public enum ShapePathType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LineTo | `1` | Segmento de línea recta |
| CubicBezierCurveTo | `3` | Curva Bézier cúbica |
| MoveTo | `0` | Inicia una nueva ruta |
| Close | `128` | Si el POINT inicial y el POINT final no son iguales, se dibuja una única línea recta para conectar el POINT inicial y el POINT final de la ruta. |
| End | `4` | El final de la ruta actual |
| Escape | `5` | Escape |
| ArcTo | `6` | Un arco |
| Unknown | `7` | Desconocido |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una forma para demostrar los tipos de ruta
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Crea una ruta de geometría personalizada
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Demuestra diferentes valores de ShapePathType
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Aplica algunas operaciones de ruta
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Guarda el libro de trabajo
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


