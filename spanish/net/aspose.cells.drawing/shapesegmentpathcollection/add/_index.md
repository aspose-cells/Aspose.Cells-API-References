---
title: "ShapeSegmentPathCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeSegmentPathCollection. Añade una ruta de segmento en la ruta de creación"
type: docs
url: /es/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Añade una ruta de segmento en la ruta de creación.

```csharp
public int Add(ShapePathType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ShapePathType | El tipo de ruta. |

### Valor de retorno

Devuelve la posición del objeto [`ShapeSegmentPath`](../../shapesegmentpath/) en la lista.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Mostrar el recuento de segmentos de ruta
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Iterar a través de cada segmento y mostrar su tipo
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //agregar forma libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Guarda el libro de trabajo para observar las modificaciones de la forma
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


