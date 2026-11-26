---
title: "ShapeSegmentPath.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeSegmentPath. Obtiene el tipo del segmento de ruta"
type: docs
url: /es/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Obtiene el tipo de segmento de ruta

```csharp
public ShapePathType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
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

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // Guarda el libro de trabajo
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


