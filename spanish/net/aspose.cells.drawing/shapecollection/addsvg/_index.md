---
title: "ShapeCollection.AddSvg"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una imagen svg"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Agrega una imagen svg.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | El desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | La altura de la forma, en unidades de píxel. |
| ancho | Int32 | El ancho de la forma, en unidades de píxel. |
| svgData | Byte[] | Los datos de la imagen svg. |
| compatibleImageData | Byte[] | Datos de imagen convertidos desde svg para ser compatibles con Excel 2016 o versiones anteriores. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // Cargar archivo SVG
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // Agregar SVG a la hoja de cálculo
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


