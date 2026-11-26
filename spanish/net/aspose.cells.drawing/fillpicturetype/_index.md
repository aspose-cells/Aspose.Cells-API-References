---
title: "Enum FillPictureType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.FillPictureType enum. Representa el tipo de relleno de imagen"
type: docs
url: /es/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Representa el tipo de relleno de imagen.

```csharp
public enum FillPictureType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Stretch | `0` | Estirar |
| Stack | `1` | Apilar |
| StackAndScale | `2` | StackAndScale |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar el relleno de imagen
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Establecer propiedades de relleno de imagen
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Utilizar una imagen mínima de 1x1 píxel (blanca) para la demostración
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Agregar otra forma con un tipo de relleno diferente
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Guardar el libro con diferentes configuraciones de relleno
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


