---
title: "MsoFormatPicture.Contrast"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la modificación de contraste de la imagen en unidades de porcentaje"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Representa la modificación de contraste de la imagen en unidades de porcentaje.

```csharp
public double Contrast { get; set; }
```

### Observaciones

Está entre -100% y 100%. Funciona igual que Excel 2007 o versiones superiores.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyContrastDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            var picture = worksheet.Pictures[pictureIndex];

            // Establecer y obtener el valor de contraste
            picture.FormatPicture.Contrast = 50;
            Console.WriteLine("Current contrast: " + picture.FormatPicture.Contrast);

            // Modificar contraste
            picture.FormatPicture.Contrast = 75;
            Console.WriteLine("Modified contrast: " + picture.FormatPicture.Contrast);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


