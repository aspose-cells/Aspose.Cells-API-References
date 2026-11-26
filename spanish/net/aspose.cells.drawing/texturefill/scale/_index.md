---
title: "TextureFill.Scale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Obtiene y establece la escala del formato de imagen"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Obtiene y establece la escala del formato de imagen.

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
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y obtener su formato de relleno
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Configurar relleno de textura
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Cargar imagen de textura y configurar propiedades
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Mostrar y modificar la escala
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Guardar resultado
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


