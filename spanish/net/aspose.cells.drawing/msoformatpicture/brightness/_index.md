---
title: "MsoFormatPicture.Brightness"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la modificación de brillo para la imagen en unidades de porcentaje"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Representa la modificación de brillo de la imagen en unidades de porcentaje.

```csharp
public double Brightness { get; set; }
```

### Observaciones

Está entre -100% y 100%. Funciona igual que Excel 2007 o versiones superiores.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // Establecer y obtener brillo
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // Modificar brillo
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


