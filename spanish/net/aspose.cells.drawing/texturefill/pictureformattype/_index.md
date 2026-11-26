---
title: "TextureFill.PictureFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Obtiene y establece el tipo de formato de imagen"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

Obtiene y establece el tipo de formato de imagen.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Establecer el tipo de relleno a textura
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Cargar imagen PNG mínima de 1x1 píxel (blanca)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // Mostrar el tipo de formato de imagen actual
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // Cambiar al formato apilado y habilitar la repetición
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // Agregar otra forma para comparar el formato original estirado
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // Guardar el libro de trabajo con ambos ejemplos de relleno de textura
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


