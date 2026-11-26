---
title: "Clase AutoNumberedBulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue. Representa viñeta numerada automática"
type: docs
url: /es/net/aspose.cells.drawing.texts/autonumberedbulletvalue/
---
## AutoNumberedBulletValue class

Representa una viñeta numerada automática.

```csharp
public class AutoNumberedBulletValue : BulletValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Representa el esquema de numeración automática. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Obtiene y establece el número inicial de la viñeta. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Obtiene el tipo de la viñeta. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassAutoNumberedBulletValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea una instancia de AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
                    StartAt = 1
                };

                // Muestra las propiedades de la viñeta
                Console.WriteLine($"Bullet Type: {bullet.Type}");
                Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
                Console.WriteLine($"Starting Number: {bullet.StartAt}");

                // Modificar propiedades
                bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
                bullet.StartAt = 5;

                // Guarda el libro de trabajo
                workbook.Save("TextsClassAutoNumberedBulletValueDemo.xlsx");
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

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


