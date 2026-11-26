---
title: "ShapeSegmentPathCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeSegmentPathCollection. Obtiene el objeto ShapeSegmentPath"
type: docs
url: /es/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Obtiene el objeto [`ShapeSegmentPath`](../../shapesegmentpath/).

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

Devuelve un objeto [`ShapeSegmentPath`](../../shapesegmentpath/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Inicia una nueva ruta
            path.MoveTo(10, 10);

            // Dibuja un segmento de línea
            path.LineTo(100, 100);

            // Acceder a la propiedad PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Mostrar el recuento de segmentos de ruta
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Demostrar la lectura de la propiedad Item
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //agregar forma libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Guarda el libro de trabajo
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


