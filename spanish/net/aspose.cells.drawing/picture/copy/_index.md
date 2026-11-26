---
title: "Picture.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Picture. Copiar la imagen"
type: docs
url: /es/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Copiar la imagen.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Imagen | La imagen fuente. |
| opciones | CopyOptions | Las opciones de copia. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insertar la primera imagen (usando una ruta de imagen de ejemplo)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Insertar segunda imagen (usando una ruta de imagen de ejemplo)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Copiar imagen 1 a imagen 2 con CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


