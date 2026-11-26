---
title: "Picture.OriginalWidthCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene el ancho original de la imagen en unidades de centímetros"
type: docs
url: /es/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

Obtiene el ancho original de la imagen, en unidades de centímetros.

```csharp
public double OriginalWidthCM { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original width of the picture in centimeters: " + pic.OriginalWidthCM);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


