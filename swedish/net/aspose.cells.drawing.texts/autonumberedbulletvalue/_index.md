---
title: "Klass AutoNumberedBulletValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue-klass. Representerar automatisk numrerad punkt"
type: docs
url: /sv/net/aspose.cells.drawing.texts/autonumberedbulletvalue/
---
## AutoNumberedBulletValue class

Representerar automatisk numrerad punkt.

```csharp
public class AutoNumberedBulletValue : BulletValue
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Representerar schemat för automatiskt nummer. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Hämtar och anger startnumret för punkten. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Hämtar typen av punkten. |

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Skapa en AutoNumberedBulletValue-instans
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
                    StartAt = 1
                };

                // Visa punktens egenskaper
                Console.WriteLine($"Bullet Type: {bullet.Type}");
                Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
                Console.WriteLine($"Starting Number: {bullet.StartAt}");

                // Ändra egenskaper
                bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
                bullet.StartAt = 5;

                // Spara arbetsboken
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

### Se även

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


