---
title: "FillFormat.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene y establece los datos de imagen"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] ImageData { get; set; }
```

### Observaciones

Si el formato de relleno no es un formato de textura personalizado, devuelve null.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen de muestra a la hoja de cálculo
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Crear un comentario y establecer los datos de imagen
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Guardar el libro de trabajo
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


