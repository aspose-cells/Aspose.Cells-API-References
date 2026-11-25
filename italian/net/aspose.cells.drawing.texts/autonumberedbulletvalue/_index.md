---
title: "Classe AutoNumberedBulletValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue classe. Rappresenta un punto elenco numerato automatico"
type: docs
url: /it/net/aspose.cells.drawing.texts/autonumberedbulletvalue/
---
## AutoNumberedBulletValue class

Rappresenta un elenco puntato numerato automatico.

```csharp
public class AutoNumberedBulletValue : BulletValue
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Rappresenta lo schema del numero automatico. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Ottiene e imposta il numero iniziale del punto elenco. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Ottiene il tipo del punto elenco. |

### Esempi

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
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea un'istanza di AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
                    StartAt = 1
                };

                // Visualizza le proprietà del punto elenco.
                Console.WriteLine($"Bullet Type: {bullet.Type}");
                Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
                Console.WriteLine($"Starting Number: {bullet.StartAt}");

                // Modifica proprietà
                bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
                bullet.StartAt = 5;

                // Salva la cartella di lavoro
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

### Vedi anche

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


