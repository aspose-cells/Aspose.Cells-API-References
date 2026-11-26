---
title: "FillFormat.TextureFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene el objeto TextureFill"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Obtiene el objeto `TextureFill`.

```csharp
public TextureFill TextureFill { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de imagen
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Establecer propiedades de relleno de textura
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Guarda el libro de trabajo
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


