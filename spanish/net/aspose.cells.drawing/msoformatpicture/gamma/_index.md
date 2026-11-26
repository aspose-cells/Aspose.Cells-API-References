---
title: "MsoFormatPicture.Gamma"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la gamma de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Representa la gamma de la imagen.

```csharp
public double Gamma { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una imagen a la hoja de cálculo (usando una ruta de imagen de ejemplo)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accede al objeto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Establecer la propiedad Gamma
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Guarda el libro de trabajo
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


