---
title: "TextureFill.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Obtiene y establece el tipo de textura"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Obtiene y establece el tipo de textura

```csharp
public TextureType Type { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular para demostrar el relleno de textura
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Establecer el tipo de relleno a textura
            shape.Fill.FillType = FillType.Texture;

            // Acceder a las propiedades de relleno de textura
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Mostrar el valor inicial de Type
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Establecer un tipo de textura diferente
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Demostrar otro tipo de textura
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Guardar el libro de trabajo para ver el efecto
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


