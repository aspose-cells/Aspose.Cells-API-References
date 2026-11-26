---
title: "MsoFormatPicture.TopCrop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación de la parte superior del rectángulo de recorte expresada como una proporción de la altura de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Representa la ubicación del borde superior del rectángulo de recorte, expresada como una proporción de la altura de la imagen.

```csharp
public double TopCrop { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Establecer la propiedad TopCrop
            picture.FormatPicture.TopCrop = -6;
            
            // Mostrar el valor de TopCrop
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Guarda el libro de trabajo
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


