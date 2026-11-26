---
title: "Picture.OriginalHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene la altura original de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Obtiene la altura original de la imagen.

```csharp
public int OriginalHeight { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Obtener y mostrar la altura original de la imagen
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

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


