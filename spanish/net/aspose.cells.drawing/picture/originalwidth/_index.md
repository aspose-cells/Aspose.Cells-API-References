---
title: "Picture.OriginalWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene el ancho original de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Obtiene el ancho original de la imagen.

```csharp
public int OriginalWidth { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Obtener y mostrar el ancho original de la imagen
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

            // Guarda el libro de trabajo
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


