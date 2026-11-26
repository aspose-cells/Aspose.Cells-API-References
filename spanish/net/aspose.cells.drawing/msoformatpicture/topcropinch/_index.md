---
title: "MsoFormatPicture.TopCropInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación de la parte superior del rectángulo de recorte expresada en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Representa la ubicación del borde superior del rectángulo de recorte, en unidades de pulgadas.

```csharp
public double TopCropInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una imagen (reemplazar con la ruta real de la imagen)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Acceder y modificar la propiedad TopCropInch
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Guardar el resultado
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


