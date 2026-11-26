---
title: "AutoNumberedBulletValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoNumberedBulletValue. Obtiene el tipo de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Obtiene el tipo de la viñeta.

```csharp
public override BulletType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para añadir texto con viñetas
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Crear un valor de viñeta autoincrementado
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Dado que no podemos establecer BulletValue directamente, necesitaremos encontrar otra forma
            // para aplicar el estilo de viñeta. Esto podría implicar usar el formato de texto de la forma
            // u otros métodos disponibles en la API.
            // Para la demostración, simplemente mostraremos el tipo de viñeta
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Agregar texto al párrafo a través del cuerpo de texto de la forma
            shape.TextBody.Text = "First Item";

            // Agregar otro párrafo con un esquema de numeración diferente
            // Dado que no podemos Add, usaremos el siguiente párrafo disponible
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Mostrar el tipo de viñeta (propiedad de solo lectura)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Agregar texto al segundo párrafo
            shape.TextBody.Text += "\nSecond Item";

            // Guardar el libro de trabajo para demostrar los efectos de la viñeta
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Ver también

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


