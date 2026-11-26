---
title: "PicFormatOption.Scale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PicFormatOption. Obtiene o establece cuántas pilas de imagen y la escala"
type: docs
url: /es/net/aspose.cells.drawing/picformatoption/scale/
---
## PicFormatOption.Scale property

Obtiene o establece cuántas imágenes se apilan y escalan.

```csharp
public double Scale { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO; // Added to resolve Stream-related issues

    public class PicFormatOptionPropertyScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una matriz de bytes de imagen BMP de 1x1 píxel
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Agregar una imagen a la hoja de cálculo usando MemoryStream
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
            Picture picture = worksheet.Pictures[pictureIndex];

            // Configurar la posición y el tamaño de la imagen
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 1;
            picture.LowerRightColumn = 1;

            // Obtener el relleno de textura a través de la propiedad FillFormat
            TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
            textureFill.PicFormatOption.Type = FillPictureType.Stack;

            // Mostrar y modificar la propiedad Scale
            PicFormatOption picFormat = textureFill.PicFormatOption;
            Console.WriteLine("Current Scale value: " + picFormat.Scale);
            picFormat.Scale = 0.5;
            Console.WriteLine("Modified Scale value: " + picFormat.Scale);

            // Expandir las dimensiones de la celda para visualizar el efecto
            worksheet.Cells.SetRowHeight(0, 100);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Guarda el libro de trabajo
            workbook.Save("PropertyScaleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


