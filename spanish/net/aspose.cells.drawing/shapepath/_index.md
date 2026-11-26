---
title: "Clase ShapePath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ShapePath. Representa una ruta de creación compuesta por una serie de movimientos, líneas y curvas que, al combinarse, formarán una forma geométrica"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Representa una ruta de creación compuesta por una serie de movimientos, líneas y curvas que, al combinarse, formarán una forma geométrica.

```csharp
public class ShapePath
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ShapePath](shapepath/)() | Inicializa una nueva instancia de la clase `ShapePath`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Obtiene la altura de esta ruta en unidades de píxeles. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsoleto.**) Obtiene la lista de [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Obtiene la lista de [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Obtiene el ancho de esta ruta en unidades de píxeles. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Añade un arco elíptico a la figura actual. El punto de inicio es el punto final de la figura actual. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Cierra la figura actual e inicia una nueva figura. Si la figura actual contiene una secuencia de líneas y curvas conectadas, el método cierra el bucle conectando una línea desde el punto final hasta el punto de inicio. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Añade una curva cúbica Bézier a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Añade un segmento de línea a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. Todos los puntos posteriores añadidos a la ruta se añaden a esta nueva figura. Unidad: Pixel. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma personalizada con todos los parámetros requeridos
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Accede a la ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Agrega una nueva ruta y accede a ella
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Muestra el número de rutas
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Guarda el libro de trabajo
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


