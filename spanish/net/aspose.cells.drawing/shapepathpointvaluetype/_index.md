---
title: "Enumeración ShapePathPointValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ShapePathPointValueType. Especifica el tipo de valor del objeto ShapePathPoint"
type: docs
url: /es/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Especifica el tipo de valor del objeto [`ShapePathPoint`](../shapepathpoint/)

```csharp
public enum ShapePathPointValueType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Position | `0` | Especifica que el tipo del objeto son coordenadas de ubicación. El objeto [`ShapePathPoint`](../shapepathpoint/) almacena los valores de coordenadas de un punto. |
| Angle | `1` | Especifica que el tipo del objeto son marcadores de ángulo. El objeto [`ShapePathPoint`](../shapepathpoint/) almacena los ángulos de inicio y fin del arco. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demostrar los valores de la enumeración ShapePathPointValueType
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Mostrar los valores del enum
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Verifique que los valores del enum coincidan con las constantes esperadas
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


