---
title: "ShapeCollection.AddIcons"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una imagen svg"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Agrega una imagen svg.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | El desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | La altura de la forma, en unidades de píxel. |
| ancho | Int32 | El ancho de la forma, en unidades de píxel. |
| imageByteData | Byte[] | Los datos de bytes de la imagen. |
| compatibleImageData | Byte[] | Datos de imagen convertidos desde svg para ser compatibles con Excel 2016 o versiones anteriores. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Crear un archivo de ícono de muestra (en uso real, usaría un archivo existente)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Agregar ícono a la hoja de cálculo
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Limpiar (opcional)
            File.Delete(iconPath);
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


