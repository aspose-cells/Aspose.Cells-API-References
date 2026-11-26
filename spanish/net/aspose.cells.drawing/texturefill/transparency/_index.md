---
title: "TextureFill.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextureFill. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 claro"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Establecer el tipo de relleno a textura
            shape.Fill.FillType = FillType.Texture;

            // Acceder a las propiedades de relleno de textura
            TextureFill textureFill = shape.Fill.TextureFill;

            // Establecer un tipo de textura incorporado
            textureFill.Type = TextureType.BlueTissuePaper;

            // Mostrar el valor inicial de transparencia
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Cambiar la transparencia al 70% (0.0 = opaco, 1.0 = totalmente transparente)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Guardar el libro de trabajo con efecto de transparencia visible
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


