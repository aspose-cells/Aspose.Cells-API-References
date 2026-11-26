---
title: "BulletValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BulletValue. Obtiene el tipo del valor de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Obtiene el tipo del valor de la viñeta.

```csharp
public abstract BulletType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear un cuadro de texto y obtener sus párrafos de texto
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Crea un valor de viñeta de carácter (que hereda de BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Mostrar el valor de la propiedad Type
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Crea un valor de viñeta de imagen para mostrar un tipo diferente
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Guarda el libro de trabajo
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


