---
title: "MsoFormatPicture.RightCrop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Representa la ubicación derecha del rectángulo de recorte expresada como una proporción del ancho de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Representa la ubicación del borde derecho del rectángulo de recorte, expresada como una proporción del ancho de la imagen.

```csharp
public double RightCrop { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
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

            // Mostrar el valor actual de RightCrop
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Establecer un nuevo valor de RightCrop (0.2 significa recortar el 20 % desde la derecha)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


