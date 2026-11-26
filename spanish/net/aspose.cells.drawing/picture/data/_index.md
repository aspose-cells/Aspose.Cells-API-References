---
title: "Picture.Data"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Obtiene los datos de la imagen.

```csharp
public byte[] Data { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insertar primera imagen
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Insertar segunda imagen
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Demostrar la propiedad Data copiando los datos de la imagen
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


