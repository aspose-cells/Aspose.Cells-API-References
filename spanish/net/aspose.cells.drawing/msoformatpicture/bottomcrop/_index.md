---
title: "MsoFormatPicture.BottomCrop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación inferior del rectángulo de recorte expresada como una proporción de la altura de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Representa la ubicación del borde inferior del rectángulo de recorte, expresada como una proporción de la altura de la imagen.

```csharp
public double BottomCrop { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Obtener el MsoFormatPicture de la imagen
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Mostrar el valor actual de BottomCrop
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Establecer un nuevo valor de BottomCrop (0.2 significa recortar el 20 % desde la parte inferior)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Establecer otros valores de recorte para demostrar el efecto
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Guardar el libro de trabajo para ver la imagen recortada
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


