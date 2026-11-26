---
title: "MsoFormatPicture.RightCropInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación del lado derecho del rectángulo de recorte expresada en pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

Representa la ubicación del borde derecho del rectángulo de recorte, en unidades de pulgadas.

```csharp
public double RightCropInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una imagen (reemplazar con la ruta real de la imagen)
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Acceder y establecer la propiedad RightCropInch
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // Guarda el libro de trabajo
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


