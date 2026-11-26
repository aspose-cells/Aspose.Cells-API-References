---
title: "ShapePath.PathSegementList"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePath. Obtiene la lista de ShapeSegmentPathCollection"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Obtiene la lista de [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/)

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ShapePath.PathSegments. Esta propiedad será eliminada 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Crear una nueva ruta de forma
                ShapePath shapePath = new ShapePath();

                // Mover al punto de inicio
                shapePath.MoveTo(10, 10);

                // Llamar al método LineTo con parámetros (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Acceder a la propiedad PathSegementList
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Mostrar el recuento de segmentos de ruta
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Iterar a través de cada segmento y mostrar su tipo
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //agregar forma libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


