---
title: "Picture.IsSameSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Picture. Devuelve si la forma es la misma"
type: docs
url: /es/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Devuelve si la forma es la misma.

```csharp
public override bool IsSameSetting(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Insertar la primera imagen (usando una ruta de imagen de ejemplo)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Insertar la segunda imagen (usando una ruta de imagen de ejemplo diferente)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Comparar la imagen consigo misma
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Comparar diferentes imágenes
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


