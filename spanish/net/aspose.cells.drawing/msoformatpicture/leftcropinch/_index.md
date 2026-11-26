---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación del lado izquierdo del rectángulo de recorte expresada en pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Representa la ubicación del borde izquierdo del rectángulo de recorte, en unidades de pulgadas.

```csharp
public double LeftCropInch { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
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

            // Establecer y obtener la propiedad LeftCropInch
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Guarda el libro de trabajo
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


