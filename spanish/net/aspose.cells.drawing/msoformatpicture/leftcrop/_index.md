---
title: "MsoFormatPicture.LeftCrop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación del lado izquierdo del rectángulo de recorte expresada como una proporción del ancho de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Representa la ubicación del borde izquierdo del rectángulo de recorte, expresada como una proporción del ancho de la imagen.

```csharp
public double LeftCrop { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Cargar datos de la imagen
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Agregar imagen a la hoja de cálculo
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // Establecer la propiedad LeftCrop
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // Obtener y establecer la propiedad LeftCropInch
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Guarda el libro de trabajo
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


