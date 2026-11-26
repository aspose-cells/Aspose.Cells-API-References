---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación inferior del rectángulo de recorte expresada en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Representa la ubicación del borde inferior del rectángulo de recorte, en unidades de pulgadas.

```csharp
public double BottomCropInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una imagen a la hoja de cálculo (usando una ruta de marcador de posición)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accede al objeto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Establecer la propiedad BottomCropInch y demostrar su uso
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Guarda el libro de trabajo
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


